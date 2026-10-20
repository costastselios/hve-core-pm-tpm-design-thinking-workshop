# Problem Domain: Three brokers, one investor

Before using Design Thinking, spend a few minutes understanding the investment domain and then experience the problem through three fictional broker apps.

You do **not** need investment expertise for this workshop. You only need enough vocabulary to understand why keeping a consolidated portfolio can be harder than simply adding together three account totals.

> **This workshop is about tracking investments, not giving investment advice.** The broker screenshots are fictional workshop mockups. Values shown inside them are fictional scenario data, not participant data.

---

# A 5-minute investing primer

## Broker

A **broker** is a service through which an investor can buy, sell, and hold investments.

An investor may use more than one broker. Each broker can know what is held on its own platform without knowing what is held somewhere else.

For this workshop, that creates the first important question:

> **If each broker only knows its own slice, where does the complete portfolio live?**

## Holding

A **holding** is an investment currently recorded as owned in the portfolio, such as shares in a company, units of an ETF, or cryptocurrency.

For a consolidated portfolio, knowing **what** is owned is not enough. The product may also need to retain **where** the holding is held.

## Stock

A **stock** represents an ownership interest in a company. A portfolio can contain stocks held across several brokers, with each broker reporting only the shares held through that platform.

## ETF

An **ETF**, or **Exchange-Traded Fund**, is an exchange-traded investment product. ETFs can themselves be holdings in an investor's portfolio even though the fund may contain many underlying investments. Investor.gov describes ETFs as exchange-traded investment products registered as investment companies or, in some cases, unit investment trusts.

For this workshop, the important idea is simply:

> **An ETF appears as one portfolio holding, even though the ETF can represent exposure to many underlying investments.**

## UCITS

**UCITS** stands for **Undertakings for Collective Investment in Transferable Securities**. It is an EU framework for collective investment funds. The European Commission describes UCITS as collective investment funds that are easily accessible by retail investors.

You may therefore encounter investments described as **UCITS ETFs**.

You do not need to understand the regulation itself for this workshop. Just recognize UCITS as a common label associated with European investment funds.

## Transaction

A **transaction** is an event recorded against an investment.

For the initial workshop scenario, the activity model focuses on:

- **Buy** — acquire more of a holding.
- **Sell** — dispose of some or all of a holding.
- **Fee** — a cost associated with investment activity.

This matters because the current quantity of a holding is connected to the activity that happened before it.

If a tracker says one quantity and new broker evidence says another, there may be missing or incorrect activity — or the historical cause may simply be unknown.

## Transaction fees

Investment activity can involve fees or commissions. Investor.gov notes that investors may encounter brokerage commissions and other fees paid to financial intermediaries, in addition to fund-level expenses.

That creates a tracking consideration: knowing quantity and transaction price may not capture every cost associated with acquiring or selling an investment.

## Dividend

A **dividend** is a distribution associated with an investment. Some investment products distribute income to investors, while some funds may reinvest income internally.

Dividends are useful background knowledge here because they illustrate a broader point:

> **A portfolio can change for reasons beyond simply buying and selling holdings.**

The workshop does not attempt to model every possible investment event.

---

# The FX problem

Now imagine investments priced in different currencies.

One holding may be priced in USD. Another may be priced in EUR. The investor may want to view the complete portfolio in AED.

Those values cannot simply be added together as if the currencies were identical.

**FX** means **foreign exchange**. An exchange rate represents the value of one currency relative to another. Investor.gov describes a foreign-currency exchange rate as the price of buying one country's currency using another country's currency.

Conceptually:

> **Holding value in reporting currency = source-currency value converted using an applicable FX rate**

That immediately raises product questions:

- Which FX rate should be used?
- From which source?
- At what point in time?
- How fresh is the rate?
- What happens if a rate is unavailable?
- Which exchange rate belongs to a historical valuation?

Do not solve those questions yet. Just notice why:

> **“Show me the total value of everything I own” is more complicated than it first appears.**

---

# The valuation problem

Different holdings can be valued using information captured at different times.

For this workshop, the product direction is toward a **factual portfolio record**, not a real-time trading screen. That makes the provenance of a value important:

- What price was used?
- What FX conversion was used?
- What was the as-of time?
- Is the information fresh, stale, unavailable, or disputed?

The key concept is **provenance**:

> **Where did this value come from, and what evidence supports it?**

---

# The gain/loss problem

Gain/loss can sound deceptively simple:

> **current value − what was invested**

But a trustworthy calculation depends on having sufficient history.

The system may need to know things such as:

- purchases;
- sales;
- quantities;
- transaction prices;
- relevant fees;
- and potentially other investment events.

Suppose the product knows:

> **“The investor owns 10 units today.”**

That may be enough to value the current holding if a usable current price is available.

It is **not necessarily enough** to say:

> **“This is exactly how much the investor gained or lost.”**

because the product may not know what those units originally cost or whether the historical activity record is complete.

This distinction becomes important later in the workshop:

> **Current-state correctness and historical completeness are not the same thing.**

A trustworthy product should be able to say:

> **“I know what is held today.”**

without pretending:

> **“I know exactly how the portfolio got here.”**

Keep that idea in mind when you reach the prototype recovery exercise.

---

# Now experience the three brokers

You now know enough terminology to examine the scenario.

As you look at each fictional broker, do **not** ask which app is best and do **not** start designing a replacement.

Instead ask:

> **What part of the investor's overall picture does this broker know?**

## Broker 1 — useful detail, narrow slice

<p align="center">
  <a href="broker-examples/broker-1/dashboard.png"><img src="broker-examples/broker-1/dashboard.png" alt="Broker 1 dashboard" width="300"></a>
  &nbsp;&nbsp;
  <a href="broker-examples/broker-1/holdings.png"><img src="broker-examples/broker-1/holdings.png" alt="Broker 1 holdings" width="300"></a>
</p>

Ask yourself:

- What can you tell about the investment held here?
- What historical context can you see?
- What could this app **not** answer about everything owned elsewhere?

## Broker 2 — another isolated holding

<p align="center">
  <a href="broker-examples/broker-2/home.png"><img src="broker-examples/broker-2/home.png" alt="Broker 2 home" width="240"></a>
  &nbsp;
  <a href="broker-examples/broker-2/holdings-value.png"><img src="broker-examples/broker-2/holdings-value.png" alt="Broker 2 holding value" width="240"></a>
  &nbsp;
  <a href="broker-examples/broker-2/holdings-shares.png"><img src="broker-examples/broker-2/holdings-shares.png" alt="Broker 2 holding shares" width="240"></a>
</p>

Ask yourself:

- What does this broker tell you about this holding?
- Is the information presented in exactly the same way as Broker 1?
- If both brokers are used, where would you look to understand the investments overall?

## Broker 3 — richer experience, still only one platform

<p align="center">
  <a href="broker-examples/broker-3/home-ytd.png"><img src="broker-examples/broker-3/home-ytd.png" alt="Broker 3 historical portfolio view" width="240"></a>
  &nbsp;
  <a href="broker-examples/broker-3/holdings.png"><img src="broker-examples/broker-3/holdings.png" alt="Broker 3 holdings list" width="240"></a>
  &nbsp;
  <a href="broker-examples/broker-3/holdings-more.png"><img src="broker-examples/broker-3/holdings-more.png" alt="Broker 3 additional holdings" width="240"></a>
</p>

Broker 3 provides a richer portfolio experience. But pause before concluding that the problem is solved.

Ask yourself:

- What can you understand here that was harder in Brokers 1 and 2?
- Does this represent **everything** owned across all brokers?
- What happens to holdings still sitting in Brokers 1 and 2?
- Where would a single historical view across all three platforms come from?

---

# Step back

Each broker can accurately describe the slice of the portfolio held on its own platform.

Even the richest broker experience still sees only its own slice.

Now carry one deceptively simple question into Design Thinking:

> ## **How do I keep track of all my holdings in one place?**

**Do not answer it yet.**

The next step is not to design a dashboard. The next step is to understand the problem.

---

## Reference sources for the primer

- [Investor.gov — Investing Basics Glossary](https://www.investor.gov/introduction-investing/investing-basics/glossary)
- [Investor.gov — ETF definition](https://www.investor.gov/introduction-investing/investing-basics/glossary/exchange-traded-fund-etf)
- [Investor.gov — Mutual Fund and ETF Fees and Expenses](https://www.investor.gov/introduction-investing/general-resources/news-alerts/alerts-bulletins/investor-bulletins/mutual-fund-and-etf-fees-and-expenses-investor-bulletin)
- [Investor.gov — Foreign Currency Exchange](https://www.investor.gov/introduction-investing/general-resources/news-alerts/alerts-bulletins/investor-bulletins/foreign)
- [European Commission — Investment funds](https://finance.ec.europa.eu/financial-markets/financial-markets-policy/investment-funds_en)
- [European Commission — UCITS Directive](https://finance.ec.europa.eu/regulation-and-supervision/financial-services-legislation/implementing-and-delegated-acts/undertakings-collective-investment-transferable-securities-directive_en)

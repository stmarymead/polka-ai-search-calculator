# The Polka — AI Search Presence Calculator

A standalone, dependency-free website to turn two manually entered Google Search Console figures into a client-ready AI Search Presence Rate.

**Live code:** `index.html` (self-contained HTML, CSS and JavaScript). **Vercel:** `vercel.json`. No build tools, database, logins, analytics, API keys or environment variables required.

## Use

1. In Google Search Console, select the client's property, date range, device and country filters.
2. Under **Performance > Search results > Web**, note **total impressions**.
3. In **Generative AI Performance > Search** (not Discover), note **impressions** for matching dates and filters.
4. Enter both numbers in the calculator; add previous-period counts to compare results.
5. Copy the summary, export CSV or print/save PDF.

Formula: `AI Search impressions ÷ total Web Search impressions × 100`.

AI Search impressions are **already included in** the Google Web Search total. This rate compares two potentially overlapping impression series. It is not share of queries, unique people, traffic, or AI recommendations. A rising ratio can happen while AI impressions decline. Always consider absolute volumes.

The form works locally in the browser. No visitor inputs are transmitted or stored by this application.

## Deploy via Vercel

In [Vercel](https://vercel.com/new), select **Add New > Project**, import `stmarymead/polka-ai-search-calculator`, choose **Other** if prompted for framework and leave the build command empty. Deploy the site as a static project. Future commits to the default branch will trigger deployments if automatic deployment is enabled.

## Reference

[Google Search Console Generative AI performance report](https://support.google.com/webmasters/answer/16984139?hl=en-GB)

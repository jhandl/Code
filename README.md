# Roadmap


## Version 2 - "Web version"
- Review pension types and minimum retirement ages (ChatGPT “Pension Types in Ireland”) 
- Add a way to view and override config settings (like DD)
- Add a link to FinSim.ie in the spreadsheet
- Add ability to fetch data from the web / google sheets
- Move the urls from the help yaml to the config file and use variables in the yaml


## Version 3 - "Modernize"
- Move core (only premium features) to backend (initially my mac, then Google functions or AWS lambda), ideally with toggle to still run in the browser for dev.
- Reimplement the UI in React
- Make things more generic so they apply to different systems

## Version 4 - "Complete"
- Add inflation volatility
- Add dividends and their tax
- Add a step function to represent government's delayed updates
- Properly handle multiple people's incomes
- Add self-employed option, joint declaration, etc
- Handle loss harvesting for trusts
- Change input system to capture the details needed for things like personal tax credits, benefits, etc.

## Version 5 - "Expand"
- Enable sharing with scenario(s) included
- Add retirement account evolving strategies (stock / bonds proportion changing over time)
- Add retirement account drawdown strategies (drawdown from bonds when stocks drop)
- Add countries and a way to select a country
- Add an event to move to a country
- Add a way for an AI agent to research a country and generate the config file for it
- Produce a log of what happened over the years (bought "cuba", sold ETF for $x, couldn't cover expenses, etc)
- Analyse the log with LLM to produce a summary of what happened and maybe some recommendations
- Add a way for the user to get an AI explanation of a point in the graph
- Highlight critical data points (depleted savings, SM crash, etc) with annotations on the graph.
- Generate PDF or Excel reports summarizing simulation results for easy sharing or record-keeping
- Add crypto because the laws in each country can be different for that (and let user select growth model - stock-to-flow, etc)
- Include features for calculating loan amortization, overpayments, and refinancing scenarios
- Add option to use historical data for the Monte Carlo simulation
- Allow user to select compare scenarios:
  - Show the graphs with a list of radio buttons to select which one to show, run on demand and draw gradually
  - Allow selecting two scenarios and add a slider to the graph to compare them (like disaster area photos)
  - Maybe rank them by success rate?
- Add a video demonstration with generated voices in different languages
- Add screen reader support and keyboard navigation for better accessibility


## Version 6 - "Monetize"
- Add a way to have EA and GA so people can test before it goes out to everyone
- Add campaigns to CIO to let people of a country know they have a new version to test (use API so it goes out as soon as the AI made changes)
- Integrate with payments provider
- Implement a tiered model:
  - Free: Basic features (save to one file, 0% volatility deterministic runs, no crypto, no log, no analysis), limited to 1 country
  - Essential: All features, limited to 1 country
  - Pro: Essential + unlimited countries
  - Premium: Pro + dedicated support
- Offer free trials to other tiers
- Offer modular upgrades (e.g., Monte Carlo add-on, country-specific tax systems).
- Add a donation button for free version users
- Add a chat box - Intercom?


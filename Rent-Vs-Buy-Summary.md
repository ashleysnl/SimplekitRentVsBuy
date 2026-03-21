# Rent vs Buy Calculator

Static SimpleKit tool for comparing the long-term financial impact of renting versus buying a home.

## What it includes

- shared SimpleKit core shell integration
- existing Google Analytics head snippet
- buy-versus-rent comparison engine
- net worth, cumulative cost, and equity-versus-investment charts
- year-by-year comparison table
- local storage and shareable URL state
- educational content, FAQ, related tools, and support CTA

## File structure

```text
/
  index.html
  assets/
    css/
      styles.css
    js/
      app.js
```

## Key assumptions in the model

- mortgage payments are calculated using the selected amortization period
- mortgage term is displayed as an assumption note only
- property taxes, insurance, fees, and flat maintenance grow with the inflation setting
- rent grows annually using the rent increase assumption
- renter investments can include avoided upfront capital and optional monthly savings when renting costs less than buying
- home equity is shown after estimated selling costs

## Local development

This is a static app. Open `index.html` in a browser or serve the repo with any simple static file server.

## Deployment

Deploy as a static site and keep these integrations intact:

- `https://core.simplekit.app/core.css`
- `https://core.simplekit.app/core.js`
- the Google Analytics snippet in `index.html`
- shared shell mount points such as `data-simplekit-header`, `data-simplekit-support`, and `data-simplekit-footer`

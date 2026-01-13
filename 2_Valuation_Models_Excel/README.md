# Valuation Model: Expand Energy Corp. (EXE)

This is a personal project where I built a valuation model for **Expand Energy Corp. (EXE)**. I wanted to create a tool that goes beyond a simple DCF by combining cash flow projections with market sentiment (Relative Valuation).

## How the model works

To get the final "Intrinsic Value," I used a blended approach (inspired by value investing strategies like Victor H's). The final price is a weighted average of two methods:

1.  **Discounted Cash Flow (66% weight):**
    I gave this the majority weight because Free Cash Flow is the most reliable metric of a company's actual performance.
2.  **Target P/E Valuation (34% weight):**
    I included this to account for how the market typically prices companies in this sector.

## Key Assumptions

Here is the reasoning behind the numbers I used in the model:

* **Target P/E Ratio (12x):**
    I didn't use the standard Forward P/E from financial news. Instead, I manually selected **12x**. Since EXE operates in the energy/commodity sector, it is cyclical and shouldn't be valued with high multiples like tech stocks (which often trade at 30x+). A multiple of 12 reflects a healthy but mature business.

* **Terminal Growth (2.5%):**
    I used 2.5% to match long-term inflation and GDP growth expectations. Assuming a higher growth rate forever (e.g., 4%) would be unrealistic for an energy company and would artificially inflate the valuation.

* **Discount Rate (8.5%):**
    Used as the WACC to discount future cash flows back to today's value.

## Usage

* **Red values:** These are manual inputs. You can download the Excel file and change the Growth Rates or Target P/E to see how the valuation changes (Sensitivity Analysis).
* **Blue values:** These are calculated fields.

---
*Note: This model is for portfolio demonstration purposes only.*

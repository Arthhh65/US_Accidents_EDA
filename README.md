# US Accidents (2016–2023) — What Makes Crashes Severe?

7.7 million accidents.  
46 features.  
3GB of raw data.  

One main question:

**What actually drives accident severity?**

This project dives deep into the US Accidents dataset to uncover patterns behind how severe accidents become — and what might influence them.

## First: Surviving the Dataset

Loading the raw CSV instantly consumed ~9.5GB of RAM.

So before doing any fancy plots, I:

- Converted repeated strings into categorical types
- Downcasted numeric columns
- Removed redundant geographic features
- Cleaned datetime columns properly

Result: Memory reduced to ~800MB.

Now the dataset behaves.

## What Did We Learn?

### Most Accidents Aren’t Catastrophic  
Severity is imbalanced — moderate levels dominate.

### No Magic Variable  
There is no single feature screaming  
“THIS causes severe accidents.”

Most linear correlations are weak.

Which means severity isn’t simple.

### Time Matters  
Severity has a noticeable negative correlation with year (-0.24).  

Over time, accidents appear slightly less severe.  
Better cars? Better roads? Better response systems?  
Probably all of the above.

### Weather Alone Isn’t the Villain  
Fog, rain, temperature — none strongly determine severity alone.
It’s likely the interaction of multiple factors that matters.

## Big Takeaway
Accident severity is messy.
It’s influenced by combinations of:
- Time
- Weather
- Infrastructure
- Geography

Which means…
A simple linear model won’t cut it.

## Future Plan
Move toward predictive modeling using:
- Class imbalance handling
- Tree-based models (Random Forest / Gradient Boosting)
- Feature interaction engineering

Because when relationships are non-linear, trees usually win.

## Stack
Python • Pandas • NumPy • Matplotlib • Seaborn

## Author
Arth Joshi  
Exploring data. Breaking assumptions. Building models next.

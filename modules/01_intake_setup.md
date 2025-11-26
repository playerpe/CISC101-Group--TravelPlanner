Update: Module 1 — Intake & Setup

Refined the intake step to improve clarity, correctness, and robustness while keeping the user experience simple.

Destination(s)

Store destinations as structured objects: { city, region/state, country }.

Support multiple destinations in the order they will be visited.

Dates or trip length (mutually exclusive)

Accept either:

Exact dates: start_date, end_date (ISO YYYY-MM-DD), or

Trip length: duration_days (positive integer).

If both are provided, resolve by prompting the user which to keep.

Number of travelers

Validate traveler_count as a positive integer (optionally track adults and children).

Reject zero or negative values with a clear error message.

Budget style

Normalize to a controlled set: budget, mid_range, luxury.

Map common synonyms (e.g., “cheap”, “backpacking”, “5-star”) to these values.

Interests

Capture user free text, but map to a controlled tag list:

e.g., food, culture, nature, shopping, nightlife, history, adventure, etc.

Allow multiple interests and store as an array.

Preferred pace

Normalize to: relaxed, balanced, fast.

Map phrases like “chill”, “slow”, “see everything”, “packed days” into these categories.

Key constraints

Categorize constraints into:

mobility (e.g., wheelchair, no long hikes)

diet (e.g., vegetarian, halal, gluten_free)

weather (e.g., avoid extreme heat, avoid rainy season)

accessibility (e.g., step-free access, elevators required)

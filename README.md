# bolt-hackathon-1
Trying out lots of things for the first time, participating in the Bolt.new hackathon!

# Restaurant Calorie Guesser (Name TBD)

*Building a calorie tracker that prioritizes mental health over obsessive precision*

## Day 1: Research Deep Dive & Project Foundation 📊

**Today's mission:** Figure out if this idea has legs, and if so, what exactly we're building.

### The Research Rabbit Hole
Spent most of the day with Perplexity, diving into calorie tracking psychology and market dynamics. The findings were pretty eye-opening:

- **71% of traditional calorie app users develop disordered eating patterns** - that's a lot of people MyFitnessPal has accidentally messed up
- **62% complain about missing restaurant data**, especially for ethnic and independent restaurants
- **Voice input shows 1.7x higher engagement** but technical implementation is a pain
- **$6.05B market growing to $17.4B by 2035** - clearly people want this to work

The research led to a strategic pivot from "general calorie tracking with AI" to "restaurant-focused calorie estimator with mindful logging features."

### What I Actually Built Today
- **Comprehensive market analysis** - two detailed research docs using academic sources and industry data
- **Voice input test app** - Web Speech API prototype that immediately failed on iPhone Safari permissions (posting it anyway for your entertainment: https://claude.ai/public/artifacts/c57f5ce0-a9bb-4e55-81c1-d2dfa5208735)
- **Project management setup** - created Claude AI assistant instructions for daily workflow management
- **Communication framework** - tone of voice guide based on [Hanna Zoon's Wordpress](https://hannazoon.wordpress.com/) for authentic, practical documentation

### Technical Decisions Made
- **Platform:** Bolt.new web app (mobile-optimized)
- **AI:** Claude Sonnet 4 for conversational food parsing  
- **Data:** USDA FoodData Central API (1,000 requests/hour, free)
- **Input method:** Text-first approach after voice permissions proved unreliable

### The Strategic Insight
Instead of competing with MyFitnessPal's 220M users, focus on the restaurant estimation gap that everyone complains about but no one solves well. Add optional "mindful mode" that hides calories during logging to address the psychological issues.

### Tomorrow's Reality Check
- Text 5-10 people about restaurant calorie estimation frustrations
- Start building the actual MVP in Bolt.new
- Test USDA API integration
- Build first conversational parser prototype

**Posted on GitHub:** Research docs, voice test app, Claude project instructions

**Evidence-based approach:** Every feature decision backed by research, not assumptions.

---

**Target:** Solve the restaurant estimation problem 62% of users struggle with  
**Days remaining:** 24

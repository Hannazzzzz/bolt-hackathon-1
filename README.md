# [Name tbd] Restaurant Calorie Estimator

AI-powered conversational tool for estimating calories at restaurants, especially independent and ethnic establishments.

## The Problem
- 62% of users complain about missing local restaurants in calorie apps
- 35-50% estimation errors for independent/ethnic restaurants
- Current apps create food obsession (71% develop disordered eating patterns)

## Our Solution
Conversational calorie estimation focused on restaurants with mindful logging approach.

## Tech Stack
- Bolt.new + React/Next.js
- Claude Sonnet 4 for conversational parsing
- USDA FoodData Central API

## Daily Progress
- **Day 1: Market research and strategic positioning** - Dove deep into the calorie tracking market and discovered the restaurant estimation gap is huge (see research files in repo). Found that 62% of users complain about missing local restaurants while existing apps focus on packaged foods and chains. Tested USDA FoodData Central API - 1,000 free requests/hour should be plenty for MVP testing. Also set up project voice guidelines and hackathon strategy docs to keep the 25-day timeline realistic. Main insight: positioning as "restaurant calorie estimator" rather than "another MyFitnessPal clone" gives us actual differentiation in a crowded market.
- **Day 2: Technical foundation and reality check** - Got the Bolt.new app working and deployed to Netlify (https://splendorous-manatee-3eb978.netlify.app/) - looks clean on mobile and the UI flows nicely. Hit a wall with Claude API costs, but the fallback estimation system actually proved our thesis perfectly: recognizes McDonald's fries easily but struggles with "croissant" or independent restaurant items. This validates exactly what our research predicted - the gap is where we thought it was. No LLM API sponsors found in hackathon docs, so we'll stick with validation using the current system and add real AI later if users want it. The broken estimator is actually better for proving market need than perfect tech right now.

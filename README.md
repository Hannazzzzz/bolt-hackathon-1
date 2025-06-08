# [Name tbd] Restaurant Nutrition Estimator

AI-powered conversational tool for estimating nutritional values at restaurants, especially independent and ethnic establishments.

## The Problem
- 62% of users complain about missing local restaurants in calorie apps
- 35-50% estimation errors for independent/ethnic restaurants
- Current apps create food obsession (71% develop disordered eating patterns)

## The Solution
Conversational calorie estimation focused on restaurants with mindful logging approach.

## Tech Stack
- Bolt.new + React/Next.js
- Claude Sonnet 4 - conversational project management and engineering coaching
- USDA FoodData Central API
- Perplexity Sonar API - conversational restaurant calorie estimation. Upgraded to 750 max_tokens for comprehensive restaurant research
- Environment variables - Secure API key management in Bolt.new
- Raw response debugging - Quality control and transparency features
- Markdown rendering - For proper formatting of AI responses

## Daily Progress
- **Day 1: Market research and strategic positioning** - Dove deep into the calorie tracking market and discovered the restaurant estimation gap is huge (see research files in repo). Found that 62% of users complain about missing local restaurants while existing apps focus on packaged foods and chains. Tested USDA FoodData Central API - 1,000 free requests/hour should be plenty for MVP testing. Also set up project voice guidelines and hackathon strategy docs to keep the 25-day timeline realistic. Main insight: positioning as "restaurant calorie estimator" rather than "another MyFitnessPal clone" gives us actual differentiation in a crowded market.
- **Day 2: Technical foundation and reality check** - Got the Bolt.new app working and deployed to Netlify (https://splendorous-manatee-3eb978.netlify.app/). Hit a wall with Claude API integration, but the fallback data-based estimation system actually proved the thesis: recognizes McDonald's fries easily but struggles with more exotic restaurant items. No LLM API sponsors found in hackathon docs, so we'll stick with validation using the current system and add real AI later. 
- **Day 3: Working AI integration and user validation** - Major breakthrough: got Perplexity API working in the app for real restaurant calorie estimation! It successfully recognized "Halle Berry from Halifax" as a milkshake from Copenhagen burger chain, proving the local restaurant knowledge works. Added quality checking features: raw AI response display and requirement for restaurant/city/menu item confirmation. Found some accuracy gaps (Lagkagehuset croissant gave 100g calories instead of actual portion size) but the core concept is validated. Also got enthusiastic user validation from friend who wants to test future prototypes. Posted blog restart announcement to document the journey: https://hannazoon.wordpress.com/2025/06/07/back-to-building-and-blogging/. Ready for tomorrow's prompt refinement to improve portion size reasoning.
- **Day 4: Restaurant context breakthrough + user psychology goldmine** - I finally got the Perplexity integration working properly by bumping the token limit to 750 - now when someone types "croissant from Lagkagehuset" it actually gives realistic portion estimates (280 calories) instead of confusing per-100g data. The restaurant research is working much better, though I'm still tweaking how it handles specific weights like "mini croissant (48g)". But the real breakthrough today was user feedback - talked to three people and discovered there are actually distinct user types who all want restaurant calorie help but can't stand traditional tracking apps. One person with eating disorder history said it "has potential" but avoids anything calorie-focused, another guy wants insights without obsessive counting, and the Slow Carb Reddit community specifically avoids calorie tracking but needs restaurant guidance. I'm realizing we might be solving a much bigger psychology problem than I initially thought - curious to test this delayed visibility approach with more people who've been burned by MyFitnessPal-style apps.

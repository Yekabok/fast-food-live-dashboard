# Scoring and Confidence Model

## Purpose
Define how recent ratings are turned into dashboard signals.

## Working approach for MVP
- accept structured user ratings across four dimensions
- aggregate ratings only within the selected time window
- default dashboard window is 15 minutes
- calculate a store-level score for each metric
- calculate a confidence level based on recent rating volume

## Suggested MVP confidence bands
- Low confidence: very small number of recent ratings
- Medium confidence: enough ratings for directional trust
- High confidence: substantial recent rating volume

## Notes
Detailed formulas are still to be defined. The product should avoid implying false precision until scoring methodology is validated.

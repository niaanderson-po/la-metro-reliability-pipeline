# LA Metro Reliability Pipeline – Design Document

**Author(s):** Nia Anderson
**Reviewer(s):** None
**Status:** Draft
**Last Updated:** 2026-02-03
**Created:** 2026-02-03

## Problem:

Transit riders in Los Angeles have no reliable way to know which Metro routes are historically underperforming. Without this context, riders waste time waiting for late trains or buses, miss connections, and in the worst case, miss events entirely, having to turn around to go home.

## Solution:

A data pipeline that ingests raw LA Metro GTFS schedule and performance data, models it into a clean star schema, and produces four analytical outputs: worst delay routes ranked by severity, a reliability score per route, a stop-level delay heatmap dataset, and a rolling on-time rate trend. This gives riders, developers, and analysts the historical context they need to make informed decisions.

## End Consumers:

A transit analyst exploring performance patterns, a developer building a rider-facing application (Me! App coming soon!), and any data engineer reviewing this work as an example of technical ability.


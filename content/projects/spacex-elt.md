+++
date = '2025-05-28T08:52:11+03:00'
draft = false
title = 'Spacex Elt'
description = "Built an ELT pipeline to load SpaceX data into BigQuery using Airflow."
tags = ["Python", "Singer", "Snowflake", "dbt"]
+++

![Running the script](/images/spacex.jpeg)

## What

This is an ELT pipeline that loads SpaceX launch data from the REST API into Snowflake. We do this with Singer (Python) and dbt.

## Why

I wanted to practise writing modular ELT pipelines and using cloud data warehouses. The goal was to simulate a production data ingestion system.

## How

I wrote a custom Singer tap in Python and used dbt to transform the data after it landed in Snowflake.

## Learnings

I learned how to handle rate limits, write idempotent tasks, and deal with flaky upstream data.
Biggest lesson: write small, testable components early.

https://github.com/ivanovyordan/course-data-engineering-spacex

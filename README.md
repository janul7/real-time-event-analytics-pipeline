# Real-Time Event Analytics Pipeline

A batch and streaming data engineering project that processes event data into validated, curated datasets for near-real-time reporting and downstream analytics.

## Project Overview

This project simulates a modern event-driven analytics workflow for streaming and batch data. It ingests raw event streams, processes them through layered transformations, validates data quality, and publishes curated analytical outputs for downstream reporting.

The goal of this project is to demonstrate practical junior data engineering skills in:
- event-driven pipeline design
- streaming and batch processing
- data validation
- layered data architecture
- analytics-ready dataset creation
- reproducible local pipeline development

## Business Problem

Organizations that depend on digital products, user interactions, or machine-generated events often need faster visibility into activity than traditional batch pipelines can provide. Raw event streams are noisy, fast-moving, and rarely suitable for analytics without cleaning and validation.

This project solves that problem by building a structured event analytics workflow that:
- ingests streaming event data
- validates and standardizes raw events
- transforms event data into clean and curated layers
- supports downstream near-real-time reporting and KPI analysis
- compares streaming and batch processing trade-offs

## What This Project Demonstrates

- Event-driven pipeline design
- Kafka-based ingestion
- PySpark transformation workflows
- Layered raw, cleaned, and curated processing
- Batch and streaming analytics patterns
- Event quality validation
- Reproducible local development with Docker

## Architecture

Event Producer -> Kafka -> PySpark Processing -> Raw Layer -> Cleaned Layer -> Curated Layer -> Aggregate Outputs -> Reporting

## Tech Stack

- Python
- SQL
- Kafka
- Spark / PySpark
- Docker
- Git / GitHub

## Datasets

- Event stream generator: `<dataset-link-or-generator-description>`
- Product or session reference data: `<dataset-link>`
- Reporting reference data: `<dataset-link>`

## Key Features

- Streaming ingestion of raw event data
- Batch-style aggregations for downstream reporting
- Layered event processing workflow
- Schema validation and event quality checks
- Curated analytical outputs for downstream use
- Comparison of streaming and batch processing trade-offs

## Data Model

Example analytical outputs included in this project:
- `raw_events`
- `cleaned_events`
- `curated_event_metrics`
- `mart_event_volume_summary`
- `mart_usage_by_event_type`
- `mart_session_activity`

## Repository Structure

```text
real-time-event-analytics-pipeline/
├── producer/
│   └── event_generator.py
├── spark/
│   ├── streaming_jobs/
│   ├── batch_jobs/
│   └── utils/
├── kafka/
│   └── configs/
├── data/
│   ├── raw/
│   ├── cleaned/
│   └── curated/
├── docs/
├── docker-compose.yml
└── README.md

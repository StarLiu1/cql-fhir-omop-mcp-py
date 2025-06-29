# OMOP-NLP-MCP Python Server

A Python implementation of the OMOP Natural Language to SQL translation MCP server using FastMCP and the official MCP Python SDK.

## Overview

This MCP server translates natural language medical queries into OMOP-compatible SQL queries through a standardized pipeline:

1. **Natural Language to CQL Parsing** - Convert medical queries to Clinical Quality Language
2. **VSAC Integration** - Fetch value sets from the Value Set Authority Center
3. **OMOP Concept Mapping** - Map clinical terminology to OMOP concept IDs
4. **SQL Generation** - Generate optimized OMOP CDM queries

## Quick Start

### Prerequisites

- Python 3.10 or higher
- UMLS account with VSAC access
- Access to OMOP CDM database (optional for testing)

### Installation

1. **Clone and setup:**
   ```bash
   git clone <repository-url>
   cd omop-nlp-mcp-python
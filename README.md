# Smart Sync CMS

### Multi-CMS Content Operations SaaS Platform

**Product Design · Full-Stack Development · CMS Integrations · Automation**

[Website](https://smartsynccms.com) | [Affiliate Checker](https://smartsynccms.com/affiliate-checker)

---

## Overview

Smart Sync CMS is a SaaS platform I designed and developed to manage structured content across Webflow, Payload CMS, and WordPress.

The platform brings content imports, field mapping, validation, record review, API synchronization, and mobile content management into one system.

The core workflow is:

**Import → Map → Validate → Review → Sync**

Smart Sync is built around controlled data operations. Users review proposed changes before they are applied.

## The Problem

Managing hundreds of CMS records becomes difficult when content is distributed across multiple systems.

Each CMS has its own authentication, API structure, field types, validation rules, and publishing behavior.

Common challenges include:

- Importing large datasets
- Matching incoming data to existing records
- Creating and updating items safely
- Mapping complex CMS fields
- Managing product images
- Detecting invalid or duplicate data
- Reviewing changes before synchronization
- Managing content from mobile devices

Smart Sync provides one workflow for handling these operations.

---

# 1. CMS Integrations

## Webflow

Smart Sync started as a Webflow CMS management application and expanded into a multi-CMS platform.

### Webflow Integration

- Webflow Designer Extension
- Webflow API integration
- Collection and item management
- CSV and Excel imports
- Field mapping
- Create and update operations
- Slug-based record matching
- Localization workflows
- Reference and multi-reference fields
- Image management
- Draft and live content operations
- Validation and review before synchronization

### Real CMS Operation

483 Webflow CMS items were updated in a single synchronization operation during testing.

The operation included matching existing items, reviewing incoming changes, and applying updates.

## Payload CMS

Smart Sync includes a Payload CMS integration for managing structured content through API-based workflows.

### Payload Integration

- Browser-based CMS connection
- Collection discovery
- Document retrieval
- Collection field mapping
- Create and update workflows
- Data validation
- Document synchronization
- Mobile CMS workflows
- Media import workflows

Payload integration was developed alongside the VYLLY CMS project.

## WordPress

Smart Sync also supports WordPress content operations through its REST API integration.

### WordPress Integration

- WordPress site connection
- Dynamic field and schema discovery
- Content imports
- Field mapping
- Create and update workflows
- Validation before writes
- Bulk content operations
- Media handling
- WooCommerce-related workflows
- Mobile content management

The WordPress integration reuses the main Smart Sync review and synchronization approach.

---

# 2. Core Content Operations

## Import

Prepare structured content through CSV, Excel, and supported content import workflows.

## Map

Match incoming fields to the structure of the connected CMS.

## Validate

Identify missing required values, invalid data, duplicate records, and other issues before synchronization.

## Review

Separate incoming operations into records that can be created, updated, or require attention.

Users inspect the prepared changes before approving writes.

## Sync

Apply confirmed operations through the connected CMS API.

---

# 3. Desktop and Mobile

## Desktop Workspace

The desktop application provides the main workspace for content imports, mapping, validation, review, and synchronization.

## Mobile PWA

Smart Sync includes a mobile Progressive Web App for content operations outside the desktop workspace.

Mobile workflows include:

- Connected CMS access
- Content browsing and search
- Item management
- Supported create and update operations
- Mobile import workflows
- Affiliate-related workflows

---

# 4. Affiliate Scanner

### Affiliate Product URL Validation

[Affiliate Checker Website](https://smartsynccms.com/affiliate-checker)

Affiliate Scanner is a module within Smart Sync for checking product URLs used in affiliate catalogs.

It helps users review product links before relying on them in published content.

### Main Capabilities

- Bulk product URL scanning
- Product link validation
- Broken link detection
- Product availability signals
- Verification-required detection
- Manual review of uncertain results
- Batch processing
- Affiliate catalog workflows

### Supported Marketplace Workflows

- AliExpress
- Temu
- Amazon
- Etsy

### Controlled Classification

Affiliate Scanner separates results into:

- Valid
- Review
- Broken
- Verification required

A security verification page is not automatically treated as a broken product link.

Uncertain results remain available for review instead of triggering automatic destructive changes.

---

# 5. Styler

### Webflow CSS Class and Style Management

Styler is a Webflow styling and class-management module integrated into the Smart Sync ecosystem.

It works with Webflow Designer and includes a standalone workspace.

### Main Capabilities

- Webflow page and element inspection
- Element structure analysis
- CSS class and selector inspection
- Class reuse analysis
- Naming plan review
- Breakpoint and state inspection
- Style inventory
- Controlled Apply workflows
- Verification of applied changes
- Recovery and undo workflows

### Class Reuse

Styler is designed to identify compatible elements and reuse existing CSS classes where appropriate.

Its review process accounts for selector identity and potential effects on other elements or pages.

### Controlled Changes

Styler separates inspection, planning, confirmation, and application.

The goal is to avoid unintended changes to shared styles.

---

# 6. Technical Approach

Smart Sync combines several technical areas:

- Full-stack web application development
- TypeScript
- Next.js
- CMS REST APIs
- Webflow Designer integrations
- API authentication and session handling
- Data validation and mapping
- Batch processing
- Media workflows
- Progressive Web App development
- AI-assisted content preparation
- Cloud deployment
- Testing and release validation

The application uses CMS-specific integrations while maintaining a common content operation workflow.

## Design Principles

**Review before write**

Prepare and validate changes before executing CMS operations.

**Explicit control**

Users decide when confirmed changes should be applied.

**Platform-specific validation**

CMS integrations account for their respective schemas and API behavior.

**Controlled recovery**

Failures and uncertain results should be visible and recoverable rather than silently ignored.

---

# 7. My Role

I designed and developed Smart Sync CMS across:

- Product planning
- UI/UX design
- Application architecture
- Frontend development
- Backend development
- CMS integrations
- API workflows
- Validation logic
- Mobile workflows
- Testing
- Deployment

The project includes the Styler and Affiliate Scanner modules.

---

# Project Links

- [Smart Sync CMS](https://smartsynccms.com)
- [Affiliate Checker](https://smartsynccms.com/affiliate-checker)

## Source Code

The production application is maintained in a private GitHub repository.

This public repository documents the product, its capabilities, and the technical work behind it.

No production source code or credentials are included.

# Customer Management Case Study

## Table of Contents

- [Product Context](#product-context)
- [Prototype](#prototype)
- [Problem](#problem)
- [Target Users](#target-users)
- [Product Goal](#product-goal)
- [Prototype Scope](#prototype-scope)
- [Key Product Decisions](#key-product-decisions)
- [User Flow](#user-flow)
- [Edge Cases & System Dependencies](#edge-cases--system-dependencies)
- [Goals, Signals & Metrics](#goals-signals--metrics)
- [Prototype Stages](#prototype-stages)
- [What This Case Demonstrates](#what-this-case-demonstrates)
- [Related Portfolio Context](#related-portfolio-context)

## Product Context

Customer Management is a product case within the Operations Hub prototype portfolio.

It explores how internal teams can understand customer context, navigate related operational data and move into connected systems without relying on fragmented lookups across multiple tools.

The prototype brings together customer profile data, contacts, users, tickets, offers, orders, contracts, product context, invoices and connected-system handoffs in one structured internal workspace.

The case demonstrates how an internal customer workspace can support operational clarity, safer MVP delivery, role-aware access and more consistent handoffs between support, operations, commercial and product-related teams.

## Prototype

The current prototypes cover both the first unbranded product-logic stage and a more realistic MVP reconstruction.

| Prototype | Status | Link |
|---|---|---|
| Customer Management – Unbranded Prototype | Available | [Open prototype](features/customer-management/customer-management-unbranded.html) |
| Customer Management – MVP Reconstruction | Available | [Open prototype](features/customer-management/customer-management-mvp-reconstruction.html) |
| Product Vision | Planned | Coming soon |

## Problem

Internal teams often need customer context from several operational systems before they can answer a request, understand a customer situation or continue a workflow.

Relevant information may be distributed across customer master data, contact persons, portal users, tickets, offers, orders, contracts, products, invoices and external tools.

This creates several risks:

| Risk | Impact |
|---|---|
| Fragmented system switching | Internal users lose time moving between tools before they can understand the customer situation. |
| Incomplete customer context | Relevant information can be missed or interpreted without enough operational background. |
| Unclear responsibilities | Escalation paths, contacts and ownership are not always visible at the moment they are needed. |
| Knowledge-dependent handoffs | Operational follow-up can depend on individual experience rather than structured workflow support. |
| Hard-to-trace support context | Customer, user, ticket, product and billing context may not be easy to connect. |

The product challenge was to create a clearer internal customer workspace without turning the first version into a fully editable operations platform.

## Target Users

| User Group | Need |
|---|---|
| Support and Customer Service Teams | Fast access to customer context, tickets, users, product information and relevant billing or order status in order to answer requests and decide on next steps. |
| Customer Operations | A structured view of customer data, assigned users, status information and operational dependencies before triggering or continuing lifecycle workflows. |
| Billing, Sales and Account-Related Teams | Invoice, order, offer and contract context without switching between several systems for basic customer understanding. |
| Product and Delivery Stakeholders | A shared view of MVP scope, system dependencies and realistic internal workflow constraints before implementation. |
| Internal Platform Stakeholders | A clearer model for how operational customer information can become part of a broader employee-facing platform. |

## Product Goal

The product goal is to enable internal teams to understand customer context from one structured workspace and reduce fragmented lookups across systems.

The prototype aims to make customer-related information easier to find, easier to interpret and easier to hand over between teams, while keeping the initial MVP scope intentionally safe and mostly read-only.

On a broader product level, Customer Management acts as the foundation for future Operations Hub areas such as Customer Operations, Credentials & Security, Reporting, Contracts, Product Details and Tickets & Support.

## Prototype Scope

The case covers two portfolio stages: Unbranded and MVP Reconstruction.

| Stage | Covered in Prototype |
|---|---|
| Unbranded | Initial Customer Management handover logic, neutral product structure, feature-level customer entry and read-only customer information. |
| MVP Reconstruction | More realistic internal product experience with stronger customer-context navigation, connected-system handoffs, detail pages, operational patterns, breadcrumb navigation, light/dark mode and read-only default behavior. |

The prototypes are intentionally scoped around product logic, internal workflow clarity, information hierarchy and handover readiness rather than final production implementation.

### Scope by Area

| Area | Covered in Prototype |
|---|---|
| Customer Profile | Customer master data, internal contacts, status information and connected system context. |
| Contact Persons | Contact and escalation context, consolidated into the customer profile in the MVP Reconstruction. |
| Users | Portal users, user status, customer ID relationships and user-related operational context. |
| Tickets | Ticket context and ticket creation as the intentional active workflow. |
| Offers | Offer and deal context for internal commercial visibility. |
| Orders | Order context, progress, source information and operational follow-up. |
| Contracts / Products | Contract and product-related information for internal service context. |
| Invoices | Billing-related context and invoice visibility. |
| Connected Systems | Links and handoffs to external or legacy tools where deeper actions happen. |
| Adjacent Areas | Support and Reports are visible as adjacent MVP areas but not expanded in this Customer Management flow. |

## Key Product Decisions

| Decision | Rationale |
|---|---|
| Move from feature-first access to customer-context navigation | The unbranded version uses feature-level customer entry to make the initial handover logic explicit. The MVP Reconstruction shifts the experience toward a stronger customer context: internal users search once, open a customer workspace and navigate related areas from there. |
| Keep the initial scope mostly read-only | Customer Management is positioned as an internal context and navigation workspace, not as a full operational editing platform. This reduces risk, supports safer MVP delivery and makes responsibilities clearer. |
| Treat ticket creation as the intentional active workflow | Most areas remain read-only, but ticket creation remains active because it represents a common internal handoff from customer context into support work. |
| Consolidate Contact Persons into Customer Profile | The MVP Reconstruction simplifies the information architecture by moving contact-related information into the Customer Profile instead of keeping it as a separate primary area. |
| Make connected-system behavior visible | The prototype uses links, detail views, source context and handoff patterns to show where internal users need to move from Operations Hub into connected systems. |
| Show MVP boundaries explicitly | Support and Reports are visible as adjacent MVP areas but intentionally not expanded in this Customer Management flow. This keeps the prototype realistic and prevents the case from becoming too broad. |
| Use role-aware read-only patterns | Internal users may need visibility into sensitive or operationally relevant information without automatically receiving edit permissions. |

## User Flow

The prototype follows a customer-context workflow from search to operational handoff.

| Step | Description |
|---|---|
| 1. Customer Management Entry | Internal user enters the Customer Management area from Operations Hub. |
| 2. Customer Search | User searches for a customer or customer ID. |
| 3. Customer Workspace | User opens the customer workspace and sees the most important profile context. |
| 4. Context Navigation | User navigates between customer profile, users, tickets, offers, orders, contracts/products and invoices. |
| 5. Detail Inspection | User opens detail views where more operational context is needed. |
| 6. Connected-System Handoff | User follows links into connected systems when deeper action or source-system handling is required. |
| 7. Ticket Creation | User creates a ticket from customer context when support handoff is needed. |
| 8. Return to Customer Context | User can return to the customer workspace without losing the broader customer context. |

## Edge Cases & System Dependencies

The prototype includes selected internal tooling constraints and operational edge cases.

| Area | Example |
|---|---|
| Customer Not Found | Search may return no result or require a different customer identifier. |
| Multiple Customer IDs | One customer may have several related customer IDs or account contexts. |
| Inactive or Incomplete Records | Customer records may be inactive, incomplete or require additional verification. |
| Portal User Status | Assigned portal users may be active, inactive, pending or linked to multiple customer IDs. |
| Open Tickets or Escalations | Internal users need visibility into ongoing support context before taking action. |
| Billing or Invoice Issues | Unpaid, disputed or correction-related invoices may influence the customer situation. |
| Inconsistent System Data | Connected systems may not show fully aligned customer information. |
| Role-Based Visibility | Some internal users may only see selected information depending on role and access level. |
| Read-Only Sensitive Context | Sensitive or operationally relevant data may be visible but not editable in the MVP scope. |
| Connected-System Handoff | Some actions remain in source systems rather than being edited directly in Operations Hub. |
| Adjacent Workflow Scope | Support and reporting workflows are visible but remain outside the Customer Management MVP scope. |

These dependencies are intentionally reflected in the prototypes to support better discussion between product, design, development, operations, support and business stakeholders.

## Goals, Signals & Metrics

The prototype is framed around internal product outcomes rather than screens alone.

The main goal is to reduce fragmented customer lookups and help internal teams understand customer context faster, more safely and with clearer operational handoffs.

| Goal | Signal | Potential Metrics |
|---|---|---|
| Improve access to customer context | Internal users can search for a customer and open related profile, user, ticket, order, product and invoice context from one workspace. | Time to find customer context, search success rate, number of customer lookups completed without switching systems. |
| Reduce fragmented system switching | Frequently needed customer information is available in one structured view, while deeper actions use clear connected-system handoffs. | Number of systems opened per support case, handoff link usage, reduction in manual cross-system lookups. |
| Increase confidence in customer information | Users can see customer master data, responsibilities, contacts, related users, status information and operational context in one place. | Completeness of customer context, number of clarification requests, user confidence rating in internal feedback. |
| Support faster support and service handling | Tickets, users, product context and invoice/order information are accessible from the same customer context. | Average handling time, first-contact resolution rate, time from customer lookup to support action. |
| Keep MVP scope safe and controllable | Most areas remain read-only, while ticket creation is the intentional active workflow. | Number of unintended data changes, audit issues, permission-related incidents, scope change requests. |
| Improve internal handover quality | Product, design, development and operations can discuss customer management scope, system dependencies and MVP boundaries from the same prototype. | Number of clarified requirements before implementation, reduced rework, stakeholder review feedback, documented edge cases. |
| Make future evolution visible | Adjacent areas such as Support and Reports are visible without overloading the Customer Management MVP. | Number of validated follow-up ideas, prioritization clarity, roadmap items derived from stakeholder feedback. |

These metrics are intentionally defined as potential indicators. The prototype does not measure them directly, but uses them to frame what a successful implementation would need to improve: customer context access, internal efficiency, operational reliability and handover quality.

## Prototype Stages

The Customer Management case is intended to evolve across three prototype stages.

| Stage | Focus |
|---|---|
| Unbranded | Initial handover concept focused on customer data structure, feature-level entry points, read-only customer context and basic operational navigation. |
| MVP Reconstruction | More realistic internal product reconstruction with customer-context search, detail views, connected-system handoffs, breadcrumb navigation, realistic MVP boundaries and read-only default behavior. |
| Product Vision | Future-oriented expansion toward stronger governance, auditability, role-based personalization, proactive risk indicators, lifecycle operations and cross-area reporting. |

These iterations move the prototype from an initial internal customer overview toward a broader Operations Hub customer workspace.

## What This Case Demonstrates

This case highlights the product capabilities behind the Customer Management prototype.

| Capability | Evidence in this case |
|---|---|
| Internal platform product thinking | Connects customer profile, users, tickets, offers, orders, contracts, products, invoices and system handoffs into one internal workspace. |
| Employee experience design | Reduces fragmented lookups and helps internal users build customer context faster. |
| Information architecture | Structures complex customer and operational data into understandable areas and navigation patterns. |
| MVP scoping | Keeps the first implementation mostly read-only while making ticket creation the intentional active workflow. |
| Operational realism | Reflects incomplete data, multiple customer IDs, role-based visibility, connected-system handoffs and MVP boundaries. |
| Workflow and handover design | Supports movement from customer context into support, operational and connected-system follow-up. |
| Outcome-oriented product thinking | Defines goals, signals and potential metrics around context access, system switching, confidence, handling time and handover quality. |
| Product evolution | Moves from unbranded handover logic toward a more realistic internal platform reconstruction and future product vision. |

## Related Portfolio Context

Customer Management is one product area within the broader Operations Hub prototype portfolio.

It connects to other planned Operations Hub areas such as Customer Operations, Credentials & Security, Reporting, Contracts & Product Details and Tickets & Support.

Within the wider portfolio, Customer Management has a specific role:

- Customer Portal demonstrates customer-facing self-service and product journeys.
- Operations Hub demonstrates employee-facing operational workflows and internal platform thinking.
- Customer Management acts as the foundation for understanding internal customer context before operational actions or lifecycle workflows happen.

The case is especially relevant for roles focused on internal platforms, employee experience, service operations, customer operations, workflow design, product discovery, information architecture and complex B2B platform environments.

---
title: Mar y Bosque - Tour Booking Platform
description: A modern, responsive web platform for managing tour reservations, experiences, and hostel services in Bahía Drake, Costa Rica.
pubDate: 2026-01-10
heroImage: ../../assets/proyecto1.png
tags: ["JavaScript", "HTML", "CSS", "Bootstrap", "Google Sheets"]
---

[Mar y Bosque](https://github.com/CorcovadoCodeStudio/marybosque_proyecto) is a full-featured booking platform built for a real tourism and hostel business in Bahía Drake, Costa Rica — one of the most remote and biodiverse regions on the planet.

The platform handles the entire reservation flow: from browsing a tour catalogue with multiple modalities and pricing, to a step-by-step booking form with email verification via a 6-digit code. Once confirmed, reservations are stored in Google Sheets through a Google Apps Script webhook, keeping operations lightweight and accessible for a non-technical team.

On the admin side, the dashboard provides full control: filter bookings by name, email, date, status, or operator; approve, reject, or delete entries; and track live stats across pending and confirmed reservations.

## What I built

- A complete client-facing booking flow with modality selection, date picking, and email verification (EmailJS)
- An admin dashboard with advanced filters, bulk actions, and reservation statistics
- A JSON-driven tour catalogue (`tours.json`) making content updates straightforward
- Scroll-reveal animations and a fully responsive layout optimized for mobile tourists in the field

## Stack

The project runs entirely client-side — no heavy framework, no backend server. HTML5, CSS3, and Vanilla JavaScript keep it fast and deployable anywhere. Bootstrap 5 handles the responsive grid, and Google Apps Script acts as a serverless backend connecting form submissions to a Google Sheets database.

## Team

Built collaboratively with **Alberto Acebes Sánchez** and **Mikel Franco Santana** as part of a real-world deployment for the Mar y Bosque business.
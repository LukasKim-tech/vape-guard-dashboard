# Vape Guard — Dashboard

Live cigarette smoke monitoring for a dorm room, built on an ESP32 with an SGP30
air quality sensor.

**https://lukaskim-tech.github.io/vape-guard-dashboard/**

## Signing in

The dashboard needs an account. The first person to open it creates the admin
account; after that, admins add everyone else from Settings → People. There is
no public sign-up.

Sessions last 14 days.

## What it shows

The page leads with one word — **Clear**, **Elevated**, **Warning**, **Smoke** —
because that is the only thing worth knowing at a glance. The background is the
reading itself: a field of drifting particles that stays almost colourless at
rest and turns turbulent and red the moment smoke is detected.

Below that: eCO₂, the learned baseline, today's peak, today's alarms, and device
uptime, then the last 200 readings and a log of the last 20.

Admins can also restart the device, trigger a test alarm, or make the sensor
relearn its baseline.

## Security

The Apps Script URL is in this page, which is fine: reading data and controlling
the device both require a session token, so the URL alone grants nothing.
Passwords are stored salted and hashed, never in the clear. The device
authenticates separately with its own token.

## Source

This repository holds only the dashboard. The firmware, backend and enclosure
live in a private repository.

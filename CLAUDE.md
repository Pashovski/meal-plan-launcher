# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

PDF-Launchers is a static, zero-dependency web page ("Pasha D Meal Plan") that displays a monthly meal plan PDF using the browser's native PDF viewer. There is no build system, no JavaScript, and no external dependencies.

## Architecture

The entire application is a single HTML file (`meal-plan-launcher.html`) that uses an `<embed>` tag to render a PDF full-screen on a dark (#1e1e1e) background. Monthly PDF files are stored alongside the HTML file in the root directory.

## How to Update the Meal Plan

1. Add the new PDF file to the root directory following the naming convention: `latest_meal_plan_<month>_<year>.pdf`
2. Update the `src` attribute of the `<embed>` tag in `meal-plan-launcher.html` to point to the new file.

## Deployment

Open `meal-plan-launcher.html` directly in a browser, or serve the directory with any static file server.

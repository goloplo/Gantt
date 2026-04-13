# Annual Gantt with Subtasks

This repository contains a single static HTML file that displays an annual Gantt chart
with support for projects, subtasks (categories), and multiple time periods per item.

## Overview

The app is a self-contained `index.html` (formerly `gantt.html`) that runs in the browser
and provides an interactive editor to add projects and subtasks, assign colors, and
define one or more time ranges for each item.

Key features:
- Add, edit and reorder projects and subtasks
- Assign multiple periods (start/end years) per project and subtask
- Export and import data via CSV
- Export visual output as JPG or XLS
- Adjustable layout and styling via toolbar controls and CSS variables

## Usage

1. Open `index.html` in a modern browser (double-click or File → Open).
2. Use the toolbar to add projects, subtasks, and define periods.
3. Adjust visual settings (column widths, font sizes, bar height, program color) using the controls.
4. Use the export buttons to download CSV, JPG, or XLS.

State (projects, categories, and display settings) is saved to the browser's `localStorage`.

## Import / Export

- `Export CSV` — downloads a CSV containing project, category and period data (includes `program_color`).
- `Import CSV` — imports projects from a CSV. The importer accepts the repo's CSV format; if the
	`program_color` header is missing the importer will fall back to the first row's `project_color`.
- `Save JPG` / `Save XLS` — export a visual snapshot of the chart.

## Customization

- Change CSS variables in the `:root` section of `index.html` to alter default colors, row heights,
	font sizes, and widths.
- Toolbar sliders and inputs update these values live and persist them to `localStorage`.

## Compatibility

- Static file — works offline in any modern browser; no server required.

## License

This project is licensed under the GNU General Public License v3.0 (GPL-3.0). See the `LICENSE` file.

---

File: `index.html` — main application file in this repository.
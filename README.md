# Asset Maintenance Management

This project provides an Odoo-based asset maintenance management module for tracking assets, scheduling maintenance work, managing technicians, and recording spare parts usage.

## Features

The module includes the following main features:

- Asset management for registering and organizing company assets
- Asset categories to classify equipment by type
- Maintenance requests for reporting issues and tracking work orders
- Technician management for assigning maintenance responsibilities
- Spare part management for tracking consumables and replacement parts
- Maintenance request reporting for printing and reviewing service records
- Automated sequence numbering for assets and maintenance requests

## Main Models

The custom addon includes these core models:

- Asset
- Asset Category
- Maintenance Request
- Spare Part
- Technician

## How to Run the Project

### Prerequisites

- Python 3.10+
- PostgreSQL
- Odoo dependencies from the requirements file

### Setup

1. Open the project folder.
2. Create and activate a virtual environment:
   - Windows:
     - `python -m venv .venv`
     - `.venv\Scripts\activate`
3. Install dependencies:
   - `pip install -r MaintenanceManagement\requirements.txt`
4. Make sure your PostgreSQL server is running and create a database for Odoo.
5. Update the Odoo configuration file at `MaintenanceManagement\odoo.conf` with your database credentials.

### Start the Server

From the project root, run:

- `python MaintenanceManagement\odoo-bin -c MaintenanceManagement\odoo.conf`

Then open your browser at:

- `http://localhost:8069`

### Install the Module

1. Log in to Odoo.
2. Go to Apps.
3. Search for "Asset Maintenance Management".
4. Click Install.

## Notes

This repository contains the Odoo base platform and a custom addon under `MaintenanceManagement/custom_addons/asset_maintenance_management`.
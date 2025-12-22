# WooCommerce Conditional Shipping and Payments

A robust WooCommerce plugin to conditionally restrict payment gateways and shipping methods based on customer billing details (specifically Country).

## Features
- **Conditional Logic**: Enable or Disable payment gateways based on customer billing country.
- **Dynamic UI**: React-based admin interface for managing conditions.
- **Checkout Support**:
  - **Classic Checkout**: Fully supported via AJAX updates.
  - **Block Checkout**: Fully supported via Store API and Batch request handling.
- **REST API**: Custom endpoints for robust data persistence.

## Installation
1. Clone the repository.
2. Run `composer install` to install PHP dependencies.
3. Run `npm install` to install JavaScript dependencies.
4. Run `npm run build` to compile the admin interface.

## Development
- **Build**: `npm run build`
- **Watch**: `npm run start`

## Testing

### Unit Tests (PHPUnit)
verifies the backend logic for country detection and gateway filtering.
```bash
vendor/bin/phpunit
```

### End-to-End Tests (Playwright)
Visually verifies the checkout flow in a browser.
```bash
# Install browsers first
npx playwright install

# Run tests headlessly
npx playwright test

# Run tests with UI (Recommended for debugging)
npx playwright test --ui
```

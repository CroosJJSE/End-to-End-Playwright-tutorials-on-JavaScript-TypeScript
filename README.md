# Playwright Tutorial Notes 📚

<details>
<summary><strong>📖 Lecture 1: Introduction to Playwright</strong></summary>

## Key Concepts

### 🔄 Auto Wait Capability
- **What**: Automatic element synchronization
- **vs Selenium**: No manual waits needed
- **Benefit**: Reduces test flakiness

### 🌐 Cross-Browser Compatibility
- **Support**: All major browsers
- **Use**: Test across various environments

### 💻 Multilingual Flexibility
- **Languages**: Java, JavaScript, TypeScript, Python, C#
- **vs Cypress**: JavaScript only

## Advanced Features

### 🔍 Tracing & Debugging
- Automatic screenshots
- Video recordings
- Logs
- **Benefit**: Debug without extra coding

### 🌐 Network Interception
- Mock API calls
- Intercept requests
- **Use**: Test edge cases

### 🍪 Browser Context Management
- Reuse cookies & sessions
- **Benefit**: Efficient test execution

### 🎯 Code Generation Tool
- Record user actions
- Generate test code
- **Benefit**: Easy utility test creation

</details>

<details>
<summary><strong>📖 Lecture 2: Browser Context & Page Fixtures</strong></summary>

## Introduction to Fixtures

### 🌐 Global Browser Fixture
- **Availability**: Automatically available for all tests
- **Access**: Browser instance without explicit declaration
- **Usage**: Pass as parameter with curly braces `{ browser }`

## Browser Context

### 🔄 Creating New Context
- **Purpose**: Fresh instance like incognito window
- **Benefit**: Clean environment without cookies/plugins
- **Method**: `browser.newContext()`
- **Properties**: Can inject cookies or proxies

### 📄 Creating New Page
- **Method**: `context.newPage()`
- **Requirement**: Must use `await` to avoid test failures
- **Purpose**: New page within the context

## Page Fixture

### ⚡ Simplified Setup
- **Auto Creation**: Default browser and page context
- **Benefit**: Start automation without explicit definitions
- **Usage**: Direct access to page object

## Code Examples

### Browser Context Test
```javascript
test('Browser Context Playwright test', async ({ browser }) => {
  const context = await browser.newContext();
  const page = await context.newPage();
  await page.goto("https://rahulshettyacademy.com/loginpagePractise/");
});
```

### Page Fixture Test
```javascript
test('Page Playwright test', async ({ page }) => {
  await page.goto("https://rahulshettyacademy.com/loginpagePractise/");
});
```

## Next Steps
- **Configuration**: Browser settings through config file
- **Advanced**: More automation techniques

</details>

<details>
<summary><strong>📖 Lecture 3: Coming Soon...</strong></summary>

*Content will be added here*

</details>

---

## Quick Navigation
- [Lecture 1](#lecture-1-introduction-to-playwright) - Introduction to Playwright
- [Lecture 2](#lecture-2-coming-soon) - Coming Soon
- [Lecture 3](#lecture-3-coming-soon) - Coming Soon

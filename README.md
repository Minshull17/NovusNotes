# NovusNotes - Mortgage Underwriting Notes Generator

A streamlined web application for generating standardized mortgage underwriting notes. This tool helps mortgage underwriters quickly create consistent, professional notes for various stages of the application review process.

## Features

### Note Templates
The application includes pre-configured templates for:
- **First Review** - Initial application assessment with CG, Delphi, cashflow analysis, and automatic LTV calculation
- **Property Schedule** - Property portfolio overview including experience level and locations
- **Income** - Income documentation and employment details
- **Bank Statements** - Bank statement analysis with period and balance tracking
- **Accounts** - Company accounts and financial statements review
- **Credit** - Credit check results and commitment analysis
- **Valuation** - Property valuation assessment with rental income and demand analysis

### Key Capabilities
- **Live Preview** - See formatted notes as you type
- **Multi-Note Support** - Add multiple notes of different types in a single session
- **Automatic Calculations**:
  - LTV (Loan-to-Value) calculation
  - Maximum loan at 75% LTV
  - ICR (Interest Coverage Ratio) templates
- **Customer Status Tracking** - Mark customers as existing or new
- **Valuation Status** - Track valuation booking and instruction status
- **Copy to Clipboard** - Quick copy functionality with keyboard shortcut (Ctrl/Cmd+C)
- **Character Counter** - Track note length in real-time
- **Smart Formatting** - Automatic capitalization and punctuation

## Getting Started

### Requirements
- Any modern web browser (Chrome, Firefox, Safari, Edge)
- No server or installation required

### Usage

1. **Open the Application**
   - Simply open `index.html` in your web browser
   - Or deploy to any web server and access via URL

2. **Select Note Type**
   - Click one of the quick action buttons (First Review, Property Schedule, Income, etc.)
   - The form will update with relevant fields for that note type

3. **Fill in Details**
   - Complete the form fields as needed
   - Some fields auto-calculate (like LTV)
   - Use dropdowns for standardized values

4. **Add Notes**
   - Click "Add Note" to create additional notes of different types
   - Each note maintains its own form data
   - Remove notes with the "Remove" button if needed

5. **Review & Copy**
   - Check the live preview on the right side
   - Character count displays at the bottom
   - Click "Copy to Clipboard" or use Ctrl/Cmd+C to copy formatted notes

## Application Structure

The application is built as a single self-contained HTML file containing:
- HTML structure
- Embedded CSS styling
- Embedded JavaScript functionality
- No external dependencies

**File:** `index.html` (1,582 lines)

## Deployment

### Local Usage
```bash
# Simply open the file
open index.html
```

### Web Server Deployment
Upload `index.html` to any web server. The file will automatically serve as the default page.

#### GitHub Pages
1. Push to a GitHub repository
2. Enable GitHub Pages in repository settings
3. Select the main branch as source
4. Access at `https://[username].github.io/[repository-name]/`

#### Other Hosting
- Works with any static hosting service (Netlify, Vercel, AWS S3, etc.)
- No build process or server-side code required

## Features in Detail

### First Review Template
- Includes CG (Credit Grade), Delphi score, and cashflow analysis
- Transaction type (Re-mortgage, Purchase, Limited Company)
- Property type (SSCU, HMO, MUB)
- Automatic LTV calculation from loan amount and property value
- Credit profile assessment
- RN (Risk Navigator) score
- Existing customer tracking

### Valuation Template
- Rental income tracking
- Rental demand assessment (Good/Average/Poor)
- Property suitability rating
- Maximum loan calculation at 75% LTV
- ICR template generation

### Data Persistence
- Application data is saved automatically
- Customer status persists across sessions
- Template-specific data is preserved when switching between note types

## Browser Compatibility

Tested and working on:
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## Tips

- Use keyboard shortcut Ctrl+C (Cmd+C on Mac) to quickly copy notes
- Toggle between existing/new customer status for context-aware note generation
- The preview area is editable - make quick adjustments directly in the preview
- Character counter helps ensure notes meet length requirements

## Contributing

This is a single-file application for easy maintenance and deployment. When making changes:
1. Test thoroughly across different browsers
2. Maintain the embedded structure (keep HTML/CSS/JS in one file)
3. Preserve existing note templates and formatting logic

## License

[Add license information here]

## Support

For issues or questions:
- Create an issue in the repository
- Review the code comments in `index.html` for implementation details

## Version History

- **v1.0** (2026-01-04) - Initial release with 7 note templates and core functionality
- **Case-sensitive fix** (2026-01-04) - Renamed Index.html to index.html for web server compatibility

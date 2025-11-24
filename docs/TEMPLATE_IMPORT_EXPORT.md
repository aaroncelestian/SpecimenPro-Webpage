# Template Import/Export Guide

## Overview

SpecimenPro allows you to share collection templates with other users. This is perfect for:
- **Community sharing**: Share your MTG card template with other collectors
- **Team collaboration**: Ensure everyone uses the same fields for a research project
- **Template marketplace**: Build and share specialized templates
- **Backup**: Export your custom templates for safekeeping

## File Format

Templates are exported as `.specimentemplate` files containing JSON data:
- **Portable**: Works across all devices
- **Human-readable**: Can be edited in a text editor if needed
- **Validated**: Imported templates are checked for errors

## Exporting a Template

### From Template Management View

1. Open **Settings** → **Template Management**
2. Find the template you want to share
3. Tap the **share icon** (↑) next to the template
4. Choose how to share:
   - **AirDrop** to nearby users
   - **Messages** to send to friends
   - **Mail** to email the template
   - **Save to Files** for later use

### What Gets Exported

- Template name
- Collection type (Museum, Field, Lab, Custom)
- All custom fields with their types and options
- Custom photo types
- OCR enabled/disabled setting
- Creation date

### What Doesn't Get Exported

- Your actual collection data
- Photos or voice notes
- Personal information

## Importing a Template

### From Template Management View

1. Open **Settings** → **Template Management**
2. Tap **Import Template**
3. Select the `.specimentemplate` file from:
   - Files app
   - Downloads folder
   - iCloud Drive
   - Shared location

### From Files App

1. Tap on a `.specimentemplate` file
2. Choose **Open in SpecimenPro**
3. Template is automatically imported

### Duplicate Handling

If you import a template with the same name as an existing one:
- The imported template is automatically renamed (e.g., "Magic: The Gathering (2)")
- Both templates are kept
- You can rename or delete either one later

### Validation

Imported templates are validated to ensure:
- Template name is not empty
- All custom fields have valid names
- Photo types are properly defined
- No corrupted data

If validation fails, you'll see an error message explaining what's wrong.

## Use Cases

### Sharing MTG Template

**Scenario**: You've created a perfect MTG card template with all the fields you need.

**Steps**:
1. Export your "Magic: The Gathering" template
2. Share via AirDrop to your friend
3. They import it and can start cataloging cards immediately

### Research Team Collaboration

**Scenario**: Your geology lab needs everyone to use the same specimen fields.

**Steps**:
1. Create a custom template with required fields
2. Export and email to team members
3. Everyone imports the same template
4. Data is consistent across all collections

### Template Backup

**Scenario**: You've spent time customizing templates and want to back them up.

**Steps**:
1. Export each template
2. Save to iCloud Drive or external storage
3. If you ever need to restore, just import them back

## Template Structure (JSON)

```json
{
  "id": "UUID",
  "name": "Magic: The Gathering",
  "type": "museum",
  "enableOCR": true,
  "customFields": [
    {
      "id": "UUID",
      "name": "Card Name",
      "fieldType": "text",
      "isRequired": true
    },
    {
      "id": "UUID",
      "name": "Card Type",
      "fieldType": "singleSelect",
      "options": ["Creature", "Instant", "Sorcery"],
      "isRequired": false
    }
  ],
  "customPhotoTypes": [
    {
      "id": "UUID",
      "name": "Front",
      "isRequired": true
    }
  ],
  "createdAt": "2025-10-25T14:30:00Z"
}
```

## Security & Privacy

- **No personal data**: Templates only contain field definitions
- **Local validation**: Templates are checked before import
- **User control**: You choose what to import
- **No automatic sync**: Templates don't sync without your action

## Tips

1. **Name templates clearly**: Use descriptive names like "MTG Modern Collection" instead of just "Cards"
2. **Include OCR setting**: If your template benefits from OCR, enable it before exporting
3. **Test before sharing**: Create a test collection from your template to verify it works
4. **Version your templates**: Add version numbers to names (e.g., "MTG Template v2")
5. **Document custom fields**: Add notes about what each field is for

## Troubleshooting

### Import Fails

**Problem**: "Invalid template" error

**Solutions**:
- Check the file isn't corrupted
- Verify it's a `.specimentemplate` file
- Try re-downloading if received via email
- Ask the sender to re-export

### Template Doesn't Appear

**Problem**: Imported template not showing in list

**Solutions**:
- Check Template Management view
- Restart the app
- Verify import succeeded (check for success message)

### Duplicate Names

**Problem**: Multiple templates with similar names

**Solutions**:
- Rename templates to be more specific
- Delete unused duplicates
- Use version numbers in names

## Future Enhancements

Planned features:
- **Template marketplace**: Browse community templates
- **QR code sharing**: Share templates via QR codes
- **Batch import**: Import multiple templates at once
- **Template preview**: See fields before importing
- **Template ratings**: Community ratings for shared templates

## Support

For questions or issues with template import/export:
1. Check this documentation
2. Verify file format is correct
3. Test with a simple template first
4. Contact support with error messages

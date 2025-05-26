# Google AdSense Integration

This blog template is set up to use Google AdSense for monetization. Follow these steps to configure your AdSense account:

## Setup Instructions

1. **Sign up for Google AdSense**:

   - If you don't have an AdSense account, sign up at https://www.google.com/adsense/

2. **Get your Publisher ID**:

   - Once approved, you'll receive a Publisher ID that looks like `ca-pub-XXXXXXXXXXXXXXXX`

3. **Update your config.toml file**:

   - Replace the placeholder Publisher ID in `config.toml` with your actual Publisher ID:

   ```toml
   [params]
     googleAdsense = "ca-pub-XXXXXXXXXXXXXXXX"
   ```

4. **Create Ad Units**:
   - In your AdSense dashboard, create new ad units
   - Get the ad slot IDs for each ad unit you create
   - Replace the placeholder `XXXXXXXXXX` in the following files with your actual ad slot IDs:
     - `layouts/partials/adsense.html` - In-article ads
     - `layouts/partials/adsense-display.html` - Display ads

## Ad Placement

Ads are currently configured to appear in the following locations:

1. **In-article ads**: At the end of each article's content
2. **List view ads**:
   - At the top of list pages
   - Every 3 posts in list views
3. **Display ads**: Can be added to sidebars or other template locations

## Customizing Ad Placement

You can modify ad placement by editing the following files:

- `layouts/_default/single.html` - For single post pages
- `layouts/_default/list.html` - For list views and home page
- `layouts/partials/adsense.html` - In-article ad format
- `layouts/partials/adsense-display.html` - Display ad format

## Additional Resources

- [Google AdSense Help](https://support.google.com/adsense/)
- [AdSense Program Policies](https://support.google.com/adsense/answer/48182)

# .is-a.dev Domain Configuration

This file contains the configuration needed to register your custom `.is-a.dev` subdomain.

## Instructions

1. **Fork the is-a.dev repository**:
   - Go to: https://github.com/is-a-dev/register
   - Click "Fork" button

2. **Create your domain file**:
   - In your forked repo, navigate to `domains/` folder
   - Create a new file named: `YOUR-SUBDOMAIN.json`
   - Example: `adiras.json` for `adiras.is-a.dev`

3. **Copy the configuration**:
   - Copy the content from `is-a-dev-config.json` in this repository
   - Paste it into your new file in the forked repository
   - Customize if needed:
     - Change `username` to your GitHub username
     - Change `email` to your email
     - Update `CNAME` to point to your GitHub Pages URL

4. **Submit a Pull Request**:
   - Commit your changes
   - Create a Pull Request to the original is-a-dev/register repository
   - Add a title: "Add adiras.is-a.dev" (or your chosen subdomain)
   - Add a description explaining your request
   - Wait for approval (usually 1-3 days)

5. **Configure GitHub Pages**:
   - Once approved, go to your GitHub repository
   - Settings → Pages → Custom domain
   - Enter: `YOUR-SUBDOMAIN.is-a.dev`
   - Click Save
   - Wait for DNS to propagate (can take up to 24 hours)
   - Enable "Enforce HTTPS" once DNS is working

## Example Configuration

```json
{
  "owner": {
    "username": "OxAdiras",
    "email": "mr.adiras@gmail.com"
  },
  "record": {
    "CNAME": "oxadiras.github.io"
  }
}
```

## Alternative: A Records (for custom GitHub Pages)

If you want to use A records instead of CNAME:

```json
{
  "owner": {
    "username": "YOUR-GITHUB-USERNAME",
    "email": "your-email@example.com"
  },
  "record": {
    "A": [
      "185.199.108.153",
      "185.199.109.153",
      "185.199.110.153",
      "185.199.111.153"
    ]
  }
}
```

## Troubleshooting

- **DNS not resolving?** Wait 24 hours for propagation
- **HTTPS not working?** Make sure DNS is fully propagated first
- **PR rejected?** Check is-a.dev guidelines and fix any issues
- **Subdomain taken?** Choose a different subdomain name

## Resources

- is-a.dev GitHub: https://github.com/is-a-dev/register
- GitHub Pages Documentation: https://docs.github.com/en/pages
- DNS Checker: https://dnschecker.org/

## Notes

- The `.is-a.dev` domain is **free** and provided by the community
- Your subdomain must follow their naming guidelines
- Keep your configuration file for future reference
- You can update your configuration by submitting another PR

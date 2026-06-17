[Facebook Group Posts](https://apify.com/data-slayer/facebook-group-posts?fpr=data)

Extract Facebook group posts at scale without authentication or cookies. This scraper accesses publicly available group content through a cookieless architecture, eliminating the risk of account bans while delivering comprehensive post data, engagement metrics, and author profiles for competitive intelligence and community analysis.

## 📺 Video Tutorial: How it Works

[Video](https://www.youtube.com/embed/_hgn4f9N-tc?enablejsapi=1&rel=0)

---

## Key Features

🔒 **Cookieless / No Login Required** - Access public Facebook group posts without authentication, cookies, or account credentials. Zero risk of account suspension or rate limiting.

📈 **Scalable Architecture** - Extract thousands of group posts with detailed engagement metrics, reaction breakdowns, and author information in a single run.

✅ **Rich Post Data** - Capture complete post content including messages, timestamps, media attachments (images/videos), reaction counts by type (like, love, wow, haha, sad, angry, care), comment counts, share counts, and full author profiles with profile pictures.

⚡ **Fast & Reliable** - Optimized extraction engine delivers consistent results with automatic retry logic and error handling for uninterrupted data collection.

📊 **Export-Ready Formats** - Download your data instantly in JSON, CSV, or Excel format, ready for analysis in your preferred business intelligence tools, CRM systems, or spreadsheet applications.

## Use Cases

**Social Media Managers**: Monitor multiple Facebook groups to track trending topics, content performance patterns, and community engagement levels. Identify high-performing post formats and optimal posting times to inform your content strategy.

**Market Research Analysts**: Analyze audience sentiment and conversation themes across competitor groups or industry communities. Extract thousands of posts to identify emerging trends, pain points, and customer preferences for strategic planning.

**Sales & Lead Generation Teams**: Discover potential customers actively discussing relevant topics in niche Facebook groups. Export posts with author profiles to build targeted outreach lists and identify warm leads expressing specific needs or interests.

## Inputs

| Field | Type | Description |
| --- | --- | --- |
| groupId | String | The unique Facebook Group ID (e.g., 1439220986320043). Find this in the group URL after `/groups/`. |

## Outputs

**Available Formats**: JSON, CSV, Excel

**Key Data Fields**:

- `post_id` - Unique identifier for each post
- `url` - Direct link to the post
- `message` - Full text content of the post
- `timestamp` - Unix timestamp of when the post was created
- `comments_count` - Total number of comments
- `reactions_count` - Total reactions across all types
- `reactions` - Breakdown by type (like, love, wow, haha, sad, angry, care)
- `reshare_count` - Number of times the post was shared
- `author.id` - Author's unique Facebook ID
- `author.name` - Author's display name
- `author.url` - Link to author's profile
- `author.profile_picture_url` - Author's profile image URL
- `image.uri` - URL of attached image (if present)
- `image.height` / `image.width` - Image dimensions
- `video` - Video attachment data (if present)
- `external_url` - Any external links shared in the post

## How to Use

**Step 1**: Enter the target Facebook Group ID in the `groupId` field. You can find this numeric ID in the group's URL (e.g., facebook.com/groups/1439220986320043).

**Step 2**: Configure any additional parameters such as date ranges or post limits based on your data collection needs.

**Step 3**: Run the scraper and download your results in JSON, CSV, or Excel format. Data is available immediately upon completion.

## Sample Output

```
{
  "post_id": "4230362860539161",
  "type": "post",
  "url": "https://www.facebook.com/groups/boardgamecommunity/posts/4230362860539161/",
  "message": "Looking for recommendations on strategy games for 2-4 players. Preferably something with medium complexity and under 90 minutes playtime.",
  "timestamp": 1765705599,
  "comments_count": 23,
  "reactions_count": 15,
  "reshare_count": 2,
  "reactions": {
    "angry": 0,
    "care": 1,
    "haha": 0,
    "like": 12,
    "love": 2,
    "sad": 0,
    "wow": 0
  },
  "author": {
    "id": "pfbid0jTpnC5rAwPLzqpn8G2QbJgAi3u7qyXWyWfYuUokDiVukw2r5TtkfXu5QMrGDeA3Ll",
    "name": "Sarah Mitchell",
    "url": "https://www.facebook.com/sarah.mitchell.37",
    "profile_picture_url": "https://scontent.flhe6-1.fna.fbcdn.net/v/t39.30808-1/profile_pic.jpg"
  },
  "image": null,
  "video": null
}
```

## 🧩 Other Facebook Actors by Data Slayer

| Actor | What it does | Link |
| --- | --- | --- |
| Facebook Posts Scraper | Extract posts from any Facebook page | [Try it](https://apify.com/data-slayer/facebook-page-posts) |
| Facebook Page Details Scraper | Get full page profiles — followers, contact info, ratings | [Try it](https://apify.com/data-slayer/facebook-page-details) |
| Facebook Reviews Scraper | Extract customer reviews from any Facebook page | [Try it](https://apify.com/data-slayer/facebook-page-reviews) |
| Facebook Page Search Scraper | Search and discover Facebook pages by keyword | [Try it](https://apify.com/data-slayer/facebook-search-pages) |
| Facebook People Search Scraper | Search and find Facebook profiles by keyword | [Try it](https://apify.com/data-slayer/facebook-search-people) |
| Facebook Events Scraper | Discover Facebook events by keyword search | [Try it](https://apify.com/data-slayer/facebook-search-events) |
| Facebook Marketplace Listing Scraper | Extract detailed listing data from Facebook Marketplace | [Try it](https://apify.com/data-slayer/facebook-marketplace-details) |

## 💬 Feedback and Support

We actively maintain this actor and ship improvements based on user feedback. If you run into any issues or have ideas for new features:

- Create an issue on the Actor's **Issues tab** in Apify Console
- Rate the actor if it helped you — it helps others find it too
We typically respond within 24 hours.
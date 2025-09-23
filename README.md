# TikTok Web API

**TikTok Web API for bulk account registration, commenting, liking comments, and video uploading.**

This API allows you to automate TikTok workflows:  
- Bulk **account registration** (multi-geo support)  
- **Commenting** and replying to comments  
- **Liking comments** under videos  
- **Video upload** and feed management  

> ⚡ Perfect for marketing agencies, SMM teams, and automation developers.

---

## 📌 Endpoints

### 1. **Register TikTok Accounts**
- **POST** `/send` – Request verification code for email  
- **POST** `/register` – Complete account registration using verification code  

Parameters:
| Parameter     | Type   | Description |
|---------------|--------|-------------|
| email         | string | Email for registration |
| country_code  | string | Country code (e.g., `US`, `DE`) |
| proxy         | string | Proxy in format `user:pass@ip:port` |
| code          | string | Verification code (from `/send`) |

---

### 2. **Comment Management**
- **GET** `/get_comments` – Get comments under a video  
- **POST** `/post_comment` – Post a comment or reply  
- **POST** `/like_comment` – Like a comment  

---

### 3. **Video Feed**
- **GET** `/get_feed` – Fetch TikTok feed videos by geo

---

## 🚀 Quick Start

1. **Get your API key** – Contact us:  
   - Telegram: [@mrb0hdan](https://t.me/mrb0hdan)  

2. **Make a request**  
Example using cURL:
```bash
curl -X GET "https://api.yourdomain.com/get_comments?aweme_id=123456789&proxy=http://user:pass@ip:port" \
-H "api-key: YOUR_API_KEY"
```

---

## 💰 Pricing
- **Bulk registration:** pay-per-successful-registration  
- **Commenting/Liking:** pay-per-successful-action  
- Contact us for details.

---

## ⚙️ Requirements
- Proxy support (HTTP/SOCKS5)  
- API key (issued after onboarding)  
- TikTok-compatible email accounts  

---

## ⚠️ Disclaimer
This project is for **educational and research purposes only**.  
The use of this API **may violate TikTok's Terms of Service**.  
Users are **fully responsible for their own actions** when using this API.

---

## 📞 Contact
- Telegram: [@mrb0hdan](https://t.me/mrb0hdan)

## Example TikTok API Responses

This repository includes example responses from TikTok endpoints for testing and development purposes.  

- `examples/get_comments_response.json` — sample response from `/get_comments`
- `examples/post_comment_response.json` — sample response from `/post_comment`
- `examples/get_feed_response.json` — sample response from `/get_feed`
- `examples/get_comments_response.json` — same as JSON but exported as a JS object for direct use

# AI Twitter Engagement Bot

A smart Twitter bot that automatically responds to mentions and tweet replies using OpenAI's GPT model. Designed for maintaining active engagement with your audience.

## Key Features

- **Smart AI Replies**: Generates contextual responses using OpenAI GPT-3.5
- **Dual Engagement Modes**: Choose between mention responses or reply tracking
- **Rate Limit Protection**: Built-in safeguards to avoid API limits
- **Daily Usage Caps**: Prevent excessive API usage with configurable limits
- **Comprehensive Logging**: Detailed activity tracking for monitoring

## Quick Setup

1. **Install dependencies:**
```bash
pip install -r requirements.txt
```

2. **Configure environment variables** in `.env`:
```
TWITTER_API_KEY=your_twitter_api_key
TWITTER_API_SECRET=your_twitter_api_secret
TWITTER_ACCESS_TOKEN=your_access_token
TWITTER_ACCESS_TOKEN_SECRET=your_access_token_secret
TWITTER_BEARER_TOKEN=your_bearer_token
OPENAI_API_KEY=your_openai_api_key
```

3. **Run the bot:**
```bash
python main.py
```

## Project Architecture

```
├── config/              # Configuration management
├── src/
│   ├── twitter_client.py    # Twitter API interactions
│   ├── openai_client.py     # AI response generation
│   └── tweet_handler.py     # Core tweet processing logic
├── utils/
│   ├── logger.py           # Custom logging system
│   └── rate_limiter.py     # API usage control
├── logs/                  # Activity logs
└── main.py               # Application entry point
```

## Security Notes

- API credentials stored securely in environment variables
- Automatic rate limiting to prevent API abuse
- Configurable daily limits to control costs
- Comprehensive error handling and logging

## License

MIT License - feel free to modify and distribute.

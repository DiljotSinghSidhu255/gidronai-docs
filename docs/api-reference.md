# API Reference

Base URL: `https://api.gidronai.me/v1`

## Authentication
All requests require Bearer token: `Authorization: Bearer gai_your_key`

## Endpoints

### Scenes
| Method | Path | Description |
|--------|------|-------------|
| POST | /scenes | Create a new scene |
| GET | /scenes/:id | Get scene details |
| GET | /scenes | List scenes |
| DELETE | /scenes/:id | Delete a scene |

### Datasets
| Method | Path | Description |
|--------|------|-------------|
| POST | /scenes/:id/export | Export scene to dataset |
| GET | /datasets/:id | Get dataset status |
| GET | /datasets/:id/download | Download dataset |

## Rate Limits
- Free tier: 100 req/min, 1000 frames/day
- Pro: 1000 req/min, unlimited frames
- Enterprise: Custom

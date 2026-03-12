---
name: lyric-writer
description: 歌词创作技能。根据给定的主题或情感，创作适合 Suno AI 音乐生成的英文歌词，包含 lyrics 和 styles 参数。触发条件：用户要求写歌词、创作歌词、suno 歌词、English lyrics 等。
---

# Suno 歌词创作

## 输出格式

```json
{
  "lyrics": "[intro]\n(可选)引入段落\n\n[verse]\n主歌部分\n\n[chorus]\n副歌部分\n\n[bridge]\n(可选)桥段\n\n[outro]\n(可选)尾声",
  "styles": "风格描述，包含流派、情绪、速度、BPM、调性等"
}
```

## 创作要求

1. **全英文** - 所有歌词必须使用英文
2. **押韵** - 歌词需要押韵（AA BB 或 AABB 韵式）
3. **节奏感** - 考虑歌曲节奏，每行 6-12 个音节
4. **画面感** - 使用具体意象和动词
5. **情感递进** - Verse → Chorus 情感加深

## Styles 参数指南

常用风格示例：
- Pop, emotional, 120 BPM, C major
- R&B, soulful, 85 BPM, A minor
- Rock, energetic, 140 BPM, E minor
- Electronic, dreamy, 128 BPM, G major
- Acoustic, melancholy, 75 BPM, D minor
- Hip-hop, rhythmic, 90 BPM, F minor
- Country, storytelling, 110 BPM, G major
- Jazz, smooth, 120 BPM, Eb major

## 使用方式

用户给出主题、情绪或风格后，直接按上述 JSON 格式输出歌词和风格建议。

示例：
- 主题：loneliness → 输出关于孤独的英文歌词
- 风格：upbeat pop → 输出欢快流行的歌词

# Antigravity Tresor 🚀

**Antigravity IDE için profesyonel geliştirme araçları koleksiyonu**

> [Claude Code Tresor](https://github.com/alirezarezvani/claude-code-tresor) projesinden uyarlanmıştır.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 📋 İçindekiler

- [Nedir?](#-nedir)
- [Hızlı Başlangıç](#-hızlı-başlangıç)
- [Özellikler](#-özellikler)
- [Workflow Komutları](#-workflow-komutları)
- [Proje Yapısı](#-proje-yapısı)

## 🎯 Nedir?

Antigravity Tresor, Antigravity IDE için tasarlanmış profesyonel geliştirme araçları koleksiyonudur. Slash komutları, prompt şablonları ve en iyi pratikleri içerir.

### ✨ Öne Çıkan Özellikler

| Özellik | Açıklama |
|---------|----------|
| **8 Workflow Komutu** | Scaffold, review, test, docs ve daha fazlası |
| **Prompt Şablonları** | Frontend, backend ve debugging için hazır promptlar |
| **Kod Standartları** | ESLint, Prettier ve Git workflow'ları |
| **Örnek Projeler** | Gerçek dünya uygulama örnekleri |

## 🚀 Hızlı Başlangıç

### Kurulum

1. Bu repoyu klonlayın veya indirin
2. Projenizi Antigravity IDE ile açın
3. Slash komutlarını kullanmaya başlayın!

```bash
# Örnek kullanım
/scaffold react-component UserProfile --hooks --tests
/review --scope staged
/test-gen --file src/utils.ts
```

## 📦 Özellikler

### 🔧 Workflow Komutları

| Komut | Açıklama |
|-------|----------|
| `/scaffold` | Proje yapısı ve component oluşturma |
| `/review` | Kapsamlı kod incelemesi |
| `/test-gen` | Test dosyası oluşturma |
| `/docs-gen` | API dokümantasyonu |
| `/vulnerability-scan` | Güvenlik taraması |
| `/profile` | Performans analizi |
| `/commit` | Conventional commit mesajı |
| `/debt-analysis` | Teknik borç analizi |

### 🤖 Agents (Orijinal)

- `config-safety-reviewer` - Konfigürasyon güvenliği
- `test-engineer` - Test mühendisliği
- `docs-writer` - Dokümantasyon uzmanı
- `systems-architect` - Sistem mimarisi
- `security-auditor` - Güvenlik denetimi
- `performance-tuner` - Performans optimizasyonu
- `refactor-expert` - Kod yeniden yapılandırma

### 📝 Prompt Şablonları

- Frontend (React, Vue, Angular)
- Backend (API, Database, Auth)
- Debugging ve analiz
- Best practices

## 📁 Proje Yapısı

```
antigravity-tresor/
├── .agent/
│   └── workflows/          # Antigravity workflow komutları
│       ├── scaffold.md
│       ├── review.md
│       ├── test-gen.md
│       ├── docs-gen.md
│       ├── vulnerability-scan.md
│       ├── profile.md
│       ├── commit.md
│       └── debt-analysis.md
├── agents/                 # Orijinal agent tanımları
├── commands/               # Orijinal Claude Code komutları
├── prompts/                # Prompt şablonları
├── standards/              # Geliştirme standartları
├── examples/               # Örnek projeler
└── docs/                   # Dokümantasyon
```

## 📖 Kullanım Örnekleri

### Yeni Component Oluşturma

```bash
/scaffold react-component Button --hooks --tests
```

### Kod İncelemesi

```bash
/review --scope staged --checks security,performance
```

### Test Oluşturma

```bash
/test-gen --file src/api/users.ts --coverage 90
```

### Güvenlik Taraması

```bash
/vulnerability-scan --check secrets,owasp
```

## 🤝 Katkıda Bulunma

Pull request'lerinizi bekliyoruz! Lütfen [CONTRIBUTING.md](CONTRIBUTING.md) dosyasını inceleyin.

## 📄 Lisans

MIT License - Detaylar için [LICENSE](LICENSE) dosyasına bakın.

## 🙏 Teşekkürler

Bu proje [Claude Code Tresor](https://github.com/alirezarezvani/claude-code-tresor) projesi temel alınarak Antigravity IDE için uyarlanmıştır.

---

**Made with ❤️ for Antigravity IDE**
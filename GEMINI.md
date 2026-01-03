# Antigravity Tresor - Gemini için Hızlı Başlangıç 🚀

Antigravity IDE için profesyonel geliştirme araçlarını kullanmaya başlamak için bu rehberi takip edin.

## ⚡ 5 Dakikada Başlayın

### Adım 1: Projenizi Açın

Antigravity IDE'de herhangi bir proje açın. Workflow komutları otomatik olarak kullanılabilir olacaktır.

### Adım 2: İlk Komutunuzu Deneyin

```bash
# Yeni bir React component oluşturun
/scaffold react-component Button --hooks --tests
```

### Adım 3: Kodu İnceleyin

```bash
# Staged değişikliklerinizi inceleyin
/review
```

## 📋 Temel Komutlar

| Komut | Ne Yapar | Örnek |
|-------|----------|-------|
| `/scaffold` | Proje/component oluşturur | `/scaffold next-app my-project` |
| `/review` | Kod incelemesi yapar | `/review --scope staged` |
| `/test-gen` | Test dosyası oluşturur | `/test-gen --file utils.ts` |
| `/docs-gen` | Dokümantasyon oluşturur | `/docs-gen api` |
| `/commit` | Commit mesajı önerir | `/commit` |

## 🎯 Kullanım Senaryoları

### 🆕 Yeni Proje Başlatırken

```bash
# Full-stack Next.js projesi
/scaffold next-app my-app --features auth,docker,tests
```

### 🔍 PR Öncesi Kontrol

```bash
# Güvenlik ve performans kontrolü
/review --checks security,performance

# Güvenlik taraması
/vulnerability-scan
```

### 📝 Dokümantasyon

```bash
# API dokümantasyonu oluştur
/docs-gen api --format openapi

# README güncelle
/docs-gen readme
```

### 🧪 Test Yazarken

```bash
# Belirli dosya için test oluştur
/test-gen --file src/api/users.ts --coverage 90
```

## 💡 İpuçları

1. **Slash komutlarını keşfedin**: `/` yazarak mevcut komutları görün
2. **Help kullanın**: Her komut `--help` parametresi ile detaylı bilgi verir
3. **Kombinleyin**: Birden fazla komutu ardışık kullanabilirsiniz

## ❓ Sorun mu Var?

- [GitHub Issues](https://github.com/your-username/antigravity-tresor/issues) sayfasından sorun bildirin
- Dokümantasyon: [docs/](docs/) klasörünü inceleyin

---

**İyi kodlamalar! 🎉**

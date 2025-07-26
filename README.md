# .NET-6-7-Web-API-React-SPA-CI-CD
.NET 6 ve React ile geliştirilmiş tam yığın uygulama. CRUD işlemleri, Entity Framework Core ve SQLite kullanır. GitHub Actions ile CI/CD otomatikleştirilmiş; Docker ve Kubernetes üzerinde sürekli entegrasyon ve dağıtım sağlar. Modern ve etkili bir devops deneyimi sunar.

Harika! .NET ile güzel bir uygulama yazıp üzerine CI/CD pipeline kurmak hem öğrenmek hem portföyüne eklemek için çok iyi olur.

Önerim şöyle bir proje ve akış:

---

## Proje: Basit .NET 6/7 Web API + React SPA + CI/CD

### Özellikler

* Backend: .NET 6/7 Web API — CRUD işlemleri yapan bir REST API
* Frontend: React SPA — API’den veri çeken basit bir frontend
* Veri tabanı: SQLite (local kolaylık için)
* CI/CD: GitHub Actions + Docker + Kubernetes (MicroK8s veya başka)

---

### Adımlar:

#### 1. Backend (.NET Web API)

* `dotnet new webapi -n MyProjectApi`
* CRUD için örnek model: `Todo` (id, title, done)
* EF Core ile SQLite bağla
* Swagger UI ekle (kolay test için)

#### 2. Frontend (React)

* `npx create-react-app myproject-frontend`
* Basit bir Todo listesi, API ile CRUD yapacak
* Axios ile backend’e istek yapacak

#### 3. Dockerfile’lar

* Backend ve frontend için ayrı Dockerfile yaz
* Multi-stage build yaparak production için optimize et

#### 4. Kubernetes Manifestleri

* Deployment ve Service manifestleri yaz
* Backend ve frontend ayrı Pod/Deployment olacak

#### 5. CI/CD - GitHub Actions

* Push olunca:

  * .NET API build & test
  * React app build
  * Docker image build & push (DockerHub veya GHCR)
  * K8s üzerinde deployment güncelle (kubectl apply)

---

### Proje Büyüklüğü

Bu proje hem backend hem frontend’i kapsadığı için full-stack deneyimi verir, hem de gerçekçi CI/CD pratiği sağlar.

---




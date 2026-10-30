# Login Interceptor

Demo HTTP interceptor trong Angular: tự gắn token xác thực vào mọi request và xử lý lỗi 401 tập trung.

Dựng bằng Angular CLI 19.

## Chạy

```bash
npm install
npm start      # ng serve → http://localhost:4200
```

| Lệnh | Việc |
|---|---|
| `npm start` | chạy dev server, tự reload khi sửa file |
| `npm run build` | build vào `dist/` |
| `npm run watch` | build lại liên tục ở chế độ development |
| `npm test` | chạy unit test (Karma) |

## Ý chính

Interceptor đăng ký ở `app.config.ts` qua `provideHttpClient(withInterceptors([...]))`, nên không component nào phải tự thêm header.

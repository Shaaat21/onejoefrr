# Cherry Link

Cherry Link is a Flutter app and a Node/Express API for QR-based fleet rentals.

## Structure
- `lib/` Flutter app
- `backend/` Express API
- `.tools/` Local Node runtime (optional)

## Run the app
```bash
flutter pub get
flutter run -d chrome
```

## Run the API (local Node runtime)
```powershell
& \"C:\\Users\\conns197\\source\\work_time\\.tools\\node\\npm.cmd\" --prefix \"C:\\Users\\conns197\\source\\work_time\\backend\" run dev
```

## Run the API (system Node)
```bash
cd backend
npm install
npm run dev
```

## Configure env
Copy `backend/.env.example` to `backend/.env` and adjust values.

## API base URL
- Web/iOS: http://localhost:4000
- Android emulator: http://10.0.2.2:4000

## Dev shortcuts
- Mark a background check as CLEAR with `POST /pre-users/:id/decision` and `x-admin-token: dev-admin` (matches `.env`).

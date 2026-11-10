# Booksy SPA – App Android

App Android en Kotlin con Jetpack Compose, hecha para la asignatura Desarrollo de Aplicaciones Móviles de Duoc UC (2025). Proyecto en dupla de Agustín González y Benjamin Araya.

## Qué hace

- Login y registro con validaciones contra la API de prueba [DummyJSON](https://dummyjson.com).
- Guarda la sesión (token) con DataStore y la envía en cada petición con un interceptor de OkHttp.
- Perfil de usuario con foto desde cámara o galería.
- Navegación que se adapta a teléfono y tablet (Window Size Classes).

## Tecnologías

Kotlin · Jetpack Compose · Material 3 · Navigation Compose · ViewModel · Retrofit · OkHttp · Coroutines · DataStore · Coil

## Estructura

```
app/src/main/java/com/booksy/booksyspa/
├── data/
│   ├── local/        # SessionManager (DataStore)
│   └── remote/       # ApiService, RetrofitClient, AuthInterceptor y DTOs
├── repository/       # UserRepository, AvatarRepository
└── ui/
    ├── auth/         # Login y registro (pantallas + ViewModels)
    ├── profile/      # Perfil (pantalla + ViewModel)
    ├── screens/      # Inicio y navegación
    ├── components/   # Selector de imagen
    └── theme/        # Colores, tipografía y tema
```

## Cómo ejecutarlo

1. Clona el repositorio y ábrelo en Android Studio.
2. Sincroniza Gradle.
3. Ejecútalo en un emulador o teléfono con Android 7.0 (API 24) o superior.

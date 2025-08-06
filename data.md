# 🐘 Tarea 1: PostgreSQL con Docker y DataGrip

Este repositorio contiene la documentación y evidencia del proceso de instalación de PostgreSQL usando Docker, configuración en DataGrip y creación de una base de datos.

---

## 🐳 Comando para ejecutar Docker con PostgreSQL

Ejecuta el siguiente comando en la terminal:

```bash
docker run --name postgres-db -e POSTGRES_PASSWORD=admin123 -p 5432:5432 -d postgres
```

### Explicación:
- `--name postgres-db`: Nombre del contenedor.
- `-e POSTGRES_PASSWORD=admin123`: Contraseña del usuario `postgres`.
- `-p 5432:5432`: Mapea el puerto local al contenedor.
- `-d`: Ejecuta en segundo plano.
- `postgres`: Imagen oficial de PostgreSQL.

Para verificar que el contenedor está activo:

```bash
docker ps
```

---

## ⚙️ Pasos para configurar DataGrip

1. Abre DataGrip.
2. Ve a: `File > Data Sources and Drivers`.
3. Haz clic en `+` y selecciona `PostgreSQL`.
4. Completa los siguientes datos:
   - **Host:** `localhost`
   - **Port:** `5432`
   - **User:** `postgres`
   - **Password:** `admin123`
   - **Database:** `postgres`
5. Haz clic en **Test Connection**. Deberías ver: ✅ *Connection successful*.

---

## 🛠️ Creación de la base de datos desde DataGrip

1. Abre una nueva consola SQL desde la conexión `postgres@localhost`.
2. Ejecuta el siguiente comando:

```sql
CREATE DATABASE my_first_database;
```

3. Refresca el panel izquierdo para visualizar tu nueva base de datos.

---

## 📹 Evidencia en Video

🔗 [Video mostrando la instalación y configuración](https://drive.google.com/file/d/ID_DEL_VIDEO) *(Reemplazar con enlace real)*

---


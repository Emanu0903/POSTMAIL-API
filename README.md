
/*
README.md (summary):

# PostMail API

## Endpoints

- POST /users/plan
  - Body: { "userId": "1", "planId": 1 }
  - Asigna un plan de crédito: 1 → 30 envíos ($135), 2 → 40 ($160), 3 → 60 ($180)

- GET /users/:userId/credit
  - Recupera la cantidad de envíos disponibles.

- POST /users/:userId/shipments
  - Body: { name, address, phone, reference, observation }
  - Crea un nuevo envío y consume 1 unidad de crédito.

- POST /shipments/:id/package
  - Body: { desc, weight, bundles, deliverDate }
  - Agrega un paquete a un envío; consume crédito adicional según el peso (cada 3lb una unidad).

- GET /users/:userId/shipments
  - Lista todos los envíos del usuario.

- DELETE /shipments/:id
  - Elimina un envío y devuelve el crédito correspondiente por el servicio no utilizado.

```bash
npm install   # Instala las dependencias
npm start     # Inicia el servidor
```
*/

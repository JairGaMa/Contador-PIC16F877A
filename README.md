### Descripción 📋
Este proyecto implementa un contador utilizando el microcontrolador **PIC16F877A** y un display de 7 segmentos de cátodo común. El sistema permite contar de forma ascendente y descendente desde 0 hasta F (hexadecimal) mediante dos botones: uno para incrementar y otro para decrementar. Además, controla un relevador cuando el conteo llega a ciertos valores.

---

### Características 🚀
- **Microcontrolador:** PIC16F877A.  
- **Display:** 7 segmentos (cátodo común).  
- **Rango:** 0 a F en formato hexadecimal.  
- **Control:**  
  - Botón UP (RD2): Activa el modo ascendente.  
  - Botón DOWN (RD3): Activa el modo descendente.  
- **Relevador:**  
  - Activa al llegar a F (15).  
  - Desactiva al llegar a 0.  

---

### Archivos incluidos 📂
- `codigo.c` - Código fuente en C para el microcontrolador.  
- `evidenciaFoto.jpeg` - Imagen como evidencia del proyecto.  
- `evidenciaTabla.jpeg` - Tabla con datos recopilados durante las pruebas.  
- `evidenciaVideo.mp4` - Video mostrando el funcionamiento del contador.  

---

### Configuración de Hardware ⚙️
- **Puertos utilizados:**
  - `PORTB`: Control de segmentos del display.  
  - `PORTC`: Control del relevador.  
  - `PORTD`: Entradas para los botones.  
- **Configuración:**
  - `TRISB` como salida para el display.  
  - `TRISD` como entrada para botones.  
  - `TRISC` como salida para el relevador.  

---

### Funcionamiento 🛠️
1. **Inicio:**
   - El display muestra 0 al encender.  
2. **Conteo automático:**
   - Incrementa o decrementa según el botón presionado.  
3. **Control del relevador:**
   - Se activa en F (15) y se desactiva en 0.  
4. **Anti-rebote:**
   - Se usa un retardo para asegurar la lectura correcta de los botones.  

---

### Ejecución ▶️
- Compila el código en **mikroC PRO for PIC**.  
- Sube el archivo .hex al PIC16F877A.  
- Alimenta el circuito y observa el display y el relevador.

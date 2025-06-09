**Descripción del Proyecto**  
Este proyecto consiste en el diseño e implementación de una **GPU (Unidad de Procesamiento Gráfico)** en **VHDL**, capaz de generar señales de video y transmitirlas a través de una interfaz **HDMI** para visualización en un monitor o pantalla compatible.  

El diseño se ha implementado en una **FPGA**, aprovechando su capacidad para procesamiento en paralelo y generación de señales de video en tiempo real.  

---

## **🎯 Características Principales**  
✔ **Resolución soportada**:  
   - **640x480 @ 60Hz (VGA)**  
   - **1280x720 @ 60Hz (HDMI 720p)** *(opcional, dependiendo de la FPGA)*  

✔ **Interfaz HDMI** compatible con monitores estándar.  
✔ **Generación de gráficos básicos**:  
   - Líneas, rectángulos, formas geométricas simples.  
   - Texto en modo carácter (si se incluye una ROM de fuentes).  
   - Posibilidad de renderizar sprites básicos.  

## **⚙️ Requisitos de Hardware**  
- **FPGA compatible** (Xilinx Artix-7 y Cyclone IV).  
- **Conector HDMI** (se puede usar un PMOD HDMI o integrado en la placa).  
- **Fuente de alimentación** estable para la FPGA.  
- **Monitor HDMI** para visualización.  

---

## **🛠️ Instalación y Síntesis**  
### **1. Configuración del Entorno**  
- Herramientas recomendadas:  
  - **Xilinx Vivado** (para FPGAs Xilinx).  
  - **Intel Quartus** (para FPGAs Intel/Altera).  
- Asegurarse de tener los drivers adecuados para la FPGA.  

### **2. Síntesis e Implementación**  
1. Abrir el proyecto en Vivado/Quartus.  
2. Agregar los archivos VHDL en `rtl/`.  
3. Asignar los pines HDMI en `constraints/pins.xdc`.  
4. Generar el bitstream y programar la FPGA.  

### **3. Conexión HDMI**  
- Conectar la FPGA a un monitor mediante HDMI.  
- Si se usa un PMOD HDMI, verificar niveles de voltaje (generalmente 3.3V).  

---

## **🎮 Uso del Sistema**  
El sistema puede ser controlado mediante:  
- **Interfaz SPI/UART** para enviar comandos gráficos.  
- **Botones/Interruptores** en la FPGA para cambiar modos de visualización.  
- **Generación automática** de patrones (barras de color, texto, etc.).  

---

## **📊 Resultados Esperados**  
- **Señal HDMI estable** en el monitor.  
- **Renderizado de gráficos básicos** (ej: una pantalla de prueba con colores).  
- **Posibilidad de extender funcionalidad** (ej: añadir aceleración 2D).  

---

## **🔍 Referencias y Estándares**  
- **Especificación HDMI 1.4** (para codificación TMDS).  
- **Estándar VGA** (para generación de señales básicas).  
- **Documentación de la FPGA** (para restricciones de temporización).  


---

## **✉️ Contacto**  
📧 **charleesjobs78@gmail.com**  
🌐 **github.com/COMxI2C**  

--- 

**¡Gracias por tu interés en el proyecto!** 🚀

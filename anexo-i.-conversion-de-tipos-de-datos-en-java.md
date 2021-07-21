# Anexo I. Conversión de tipos de datos en Java

Tabla de conversión de Tipos de Datos Primitivos

|  |  | Tipo destino |  |  |  |  |  |  |  |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
|  |  | **boolean** | **char** | **byte** | **short** | **int** | **long** | **float** | **double** |
| **Tipo origen** | boolean | - | N | N | N | N | N | N | N |
|  | char | N | - | C | C | Cl | Cl | Cl | Cl |
|  | byte | N | C | - | CI | Cl | Cl | Cl | Cl |
|  | short | N | C | C | - | Cl | Cl | Cl | Cl |
|  | int | N | C | C | C | - | Cl | Cl\* | Cl |
|  | long | N | C | C | C | C | - | Cl\* | Cl\* |
|  | float | N | C | C | C | C | C | - | Cl |
|  | double | N | C | C | C | C | C | C | - |

 Explicación de los símbolos utilizados:

 **N:** Conversión no permitida \(un **`boolean`** no se puede convertir a ningún otro tipo y viceversa\).  
 **CI:** Conversión implícita o automática. Un asterisco indica que puede haber posible pérdida de datos.  
 **C:** Casting de tipos o conversión explícita.

El asterisco indica que puede haber una posible pérdida de datos, por ejemplo al convertir un número de tipo **`int`** que usa los 32 bits posibles de la representación, a un tipo **`float`**, que también usa 32 bits para la representación, pero 8 de los cuales son para el exponente.

En cualquier caso, las conversiones de números en coma flotante a números enteros siempre necesitarán un **Casting**, y deberemos tener mucho cuidado debido a la pérdida de precisión que ello supone.

**Reglas de Promoción de Tipos de Datos**

Cuando en una expresión hay datos o variables de distinto tipo, el compilador realiza la promoción de unos tipos en otros, para obtener como resultado el tipo final de la expresión. Esta promoción de tipos se hace siguiendo unas reglas básicas en base a las cuales se realiza esta promoción de tipos, y resumidamente son las siguientes: 

* Si uno de los operandos es de tipo **`double`**, el otro es convertido a **`double`**.
* En cualquier otro caso:
  * Si el uno de los operandos es **`float`**, el otro se convierte a **`float`**
  * Si uno de los operandos es **`long`**, el otro se convierte a **`long`**
  * Si no se cumple ninguna de las condiciones anteriores, entonces ambos operandos son convertidos al tipo **`int`**.

Tabla sobre otras consideraciones con los Tipos de Datos:

<table>
  <thead>
    <tr>
      <th style="text-align:left">Conversiones de n&#xFA;meros en Coma flotante (float, double) a enteros
        (int)</th>
      <th style="text-align:left">Conversiones entre caracteres (char) y enteros (int)</th>
      <th style="text-align:left">Conversiones de tipo con cadenas de caracteres (String)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">
        <p>Cuando convertimos n&#xFA;meros en coma flotante a n&#xFA;meros enteros,
          la parte decimal se trunca (redondeo a cero). Si queremos hacer otro tipo
          de redondeo, podemos utilizar, entre otras, las siguientes funciones:</p>
        <p></p>
        <p><b>+ Math.round(num):</b> Redondeo al siguiente n&#xFA;mero entero.</p>
        <p><b>+ Math.ceil(num):</b> M&#xED;nimo entero que sea mayor o igual a num.</p>
        <p><b>+ Math.floor(num):</b> Entero mayor, que sea inferior o igual a num.</p>
        <p>double num=3.5.</p>
        <p></p>
        <p><code>x=Math.round(num);    //  x = 4</code>
        </p>
        <p><code>y=Math.ceil(num);        // y = 4</code>
        </p>
        <p><code>z=Math.floor(num);      //  z = 3</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Como un tipo <code>char</code> lo que guarda en realidad es el c&#xF3;digo <b>Unicode</b> de
          un car&#xE1;cter, los caracteres pueden ser considerados como n&#xFA;meros
          enteros sin signo.</p>
        <p></p>
        <p>Ejemplo:</p>
        <p></p>
        <p><code>int num;</code>
        </p>
        <p><code>char c;</code>
        </p>
        <p>&lt;code&gt;&lt;/code&gt;</p>
        <p><code>num = (int) &#x2018;A&#x2019;;             //num = 65</code>
        </p>
        <p><code>c = (char) 65;               // c = &#x2018;A&#x2019; </code>
        </p>
        <p><code>c = (char) ((int) &#x2018;A&#x2019; + 1);  //c = &#x2019;B&#x2019;</code>
        </p>
      </td>
      <td style="text-align:left">
        <p>Para convertir cadenas de texto a otros tipos de datos se utilizan las
          siguientes funciones:</p>
        <p></p>
        <p><code>num=Byte.parseByte(cad):</code>
        </p>
        <p><code>num=Short.parseShort(cad);</code>
        </p>
        <p><code>num=Integer.parseInt(cad);</code>
        </p>
        <p><code>num=Long.parseLong(cad);</code>
        </p>
        <p><code>num=Float.parseFloat(cad);</code>
        </p>
        <p><code>num=Double.parseDouble(cad); </code>
        </p>
        <p></p>
        <p>Por ejemplo, si hemos le&#xED;do de teclado un n&#xFA;mero que est&#xE1;
          almacenado en una variable de tipo <code>String</code> llamada <code>cadena</code>,
          y lo queremos convertir al tipo de datos <code>byte</code>, har&#xED;amos
          lo siguiente:</p>
        <p></p>
        <p><code>byte n=Byte.parseByte(cadena);</code>
        </p>
      </td>
    </tr>
  </tbody>
</table>


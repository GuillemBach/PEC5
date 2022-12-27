# PEC5 - Ejercicio 1

1. ¿Cuáles son las principales diferencias entre formularios dirigidos por template y formularios reactivos?

  - En la siguiente tabla he recopilado las principales diferencias entre los formularios dirigidos por template y los formularios reactivos:

  |                          	| Formularios dirigidos por template                                                                                           	| Formularios reactivos                                                                                                   	|
|--------------------------	|------------------------------------------------------------------------------------------------------------------------------	|-------------------------------------------------------------------------------------------------------------------------	|
| Complegidad              	| Fáciles de usar ya que están basados en plantillas.                                                                          	| Más flexibles pero requieren más práctica ya que están basados en modelos para  proporcionarnos un mayor control.       	|
| Caso de uso              	| Implementar formularios sobre escenarios simples pero complicados para formularios complejos.                                	| Manejar escenarios complejos.                                                                                           	|
| Validación en formulario 	| Basado en directivas añadidas en el código HTML(template) por lo que el código en el  TypeScript del componente será mínimo. 	| Badaso en funciones por lo que tendrá más  código en la clase de TypeScript del componente y menos en el template HTML. 	|
| Enlace de datos          	| Utiliza el concepto de 'Two way data binding' (datos bidireccionales) usando la sintaxis de [(ngModel)].                     	| No se realiza ningún enlace de datos.                                                                                   	|
| Test                     	| Pruebas unitarias más complicadas.                                                                                           	| Pruebas unitarias más sencillas.                                                                                        	|
| Módulo a importar        	| FormsModule                                                                                                                  	| ReactiveFormsModule                                                                                                     	|
| Diseño                   	| Template - HTML                                                                                                              	| Componente - TypeScript                                                                                                 	|
| Directivas               	| ngForm                                                                                                                       	| FormBuilder, formGroup, FormGroup                                                                                       	|
| Controles                	| ngSubmit / ngModel                                                                                                           	| ngSubmit / formGroupName formControlName  FormControl                                                                   	|
| Validaciones             	| Directiva *ngIf / Directivas: MinLengthValidator, MaxLengthValidator, etc. / Atributos HTML + CSS.                           	| Validators en el componente (min, max, require,  MaxLength, etc.). / CSS.                                               	|
| Configutración           	| Menos explícita, creada por directivas.                                                                                      	| Más explícita, creada en la clase del componente TS.                                                                    	|
| Modelo de datos          	| Desestructurado                                                                                                              	| Estructurado                                                                                                            	|
| Mutabilidad              	| Immutable                                                                                                                    	| Mutable                                                                                                                 	|
| Previsibilidad           	| Asíncrona                                                                                                                    	| Síncrona                                                                                                                	|
|

**Nota:** Visualizar el contenido anterior en formato tabla en el repositorio GIT, ya que esta tabla se ha generado a través de una aplicación de terceros y al pegar el contenido se visualiza de esta forma desordenada e inlegible.

2. ¿Qué son, para qué sirven y cómo se utilizan las directivas ngModel y ngModelChange?

- ngModel:
   - Se trata de un enlace, entre algo que se tiene en la definición del componente (propiedad, método, ...) con un campo de formulario del template del componente.
   - Sirve para volcar un valor, de una propiedad del componente por ejemplo, dentro de un campo INPUT de formulario.
   - Se usa la directiva ngModel como si fuera una propiedad del campo INPUT, asignándole el valor que tenemos declarado en el componente.
- ngModelChange:
   - Es un evento que podemos usar para escuchar los cambios en las entradas del usuario en el formulario. Es la propiedad 'Output' de la directiva ngModel, por lo tanto, debemos usarla junto con ella. ngModle genera el evento NgModelChange, cada vez que cambia el modelo.
   - Ejemplo: <code><input [ngModel]="nombrePropiedad" (ngModelChange)="nombrePropiedad = $event"></code>
   - La propiedad del componente (nombrePropiedad) está vinculado al elemento de entrada mediante el enlace de propiedad ([ngModel]="nombrePropiedad"). Cualquier cambio realizado en la entrada se actualiza en el componente mediante el enlace de evento (ngModelChange)="nombrePropiedad = $event".

3. ¿Qué son, cuáles son y para qué sirven los estados en los formularios dirigidos por templates?



4. ¿Qué ventajas aportan los FormGroup en la composición de formularios?
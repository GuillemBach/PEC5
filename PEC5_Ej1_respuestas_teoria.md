# PEC5 - Ejercicio 1

1. ¿Cuáles son las principales diferencias entre formularios dirigidos por template y formularios reactivos?

  - 
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


2. ¿Qué son, para qué sirven y cómo se utilizan las directivas ngModel y ngModelChange?



3. ¿Qué son, cuáles son y para qué sirven los estados en los formularios dirigidos por templates?



4. ¿Qué ventajas aportan los FormGroup en la composición de formularios?
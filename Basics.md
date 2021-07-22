# Basics
- ```ng serve```
- Generate new component--->```ng g c componentname```
## Databinding
- Communication between typescript code and template(HTML)
	- String Interpolation
	- Propertybinding
	- Event binding
	- Two way data binding
### String Interpolation
- {{variableName}}
### Property binding
- \[attribute or property ]
- binds to typescript function or variable
### Event Binding
- (event)
- on execution of the event corresponding code is executed in the typescript
### Two way databinding
- enable the `ngModel` directive by adding the `FormsModule` to the `imports[]` array in the AppModule
- `import { FormsModule } from '@angular/forms';`
- Property+event binding
- \[(ngModel)]="property name"

## Understanding Directives
- Directives are instructions in the DOM
- They are just like components
- Directives are added by using attribute selector(inside the tag)
- Built in directives:
	- ```*ngIf="any condition/statement/function that returns true or false"```
	- else condition can be added with \<ng-template>  
	- ```[ngStyle]="{`background-color`:function/varible}"```
	- ```[ngClass]="{cssclassName:anything that returns true/false}"```
	- \*ngFor=" let name in array; let i=index (returns i as index of the array elements) "
	- 
	
	
	
	
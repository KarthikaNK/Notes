# Directives deep dive
-Attribute and structural directives
- Structural directives
	-	ngFor
	-	ngIf
	-	ngSwitch:
		-	[ngSwitch]="value"
		-	*ngSwitchCase="value1"
		-	*ngSwitchDefault
	-	Cant have more than one structural element in one element
- Attribute directives
	- [ngClass]
	- [ngStyle]
- creating directive
	- @Directive({selector:'[appHighlight]'})
	- inside class:
		- elementref inside constructor
		- inside ngoninit:elementref.nativeelement.property
	- instead of elementref use renderer
- reacting to events on the elements in which the directive sits on 
	- @HostListener('mouseenter') mouseover(eventdata:Event){setstyle here using  renderer}
- not use renderer ,even easier way ,use hostbinding
	- @HostBinding('style.backgroundcolor')  backgroundColor:string='any initial color'
	- inside hostlistener change backgrounColor property
- TemplateRef :Reference to template
- ViewContainerRef:Where template is placed

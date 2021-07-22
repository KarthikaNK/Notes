# Binding to custom properties
- Properties of one component cannot be accesed by other components by default
- To change this add a decorator ```@Input()``` in front of the property and import it from ```@angular/core```
- Can provide alias inside parenthesis ```@Input("AliasName")```
- Accesible by parent component or any component hosting our component
# Binding to custom events
- ```@Output()```
- Inform parent component that something changed
- Listen to event and execute anything(parent component)
- Assign new Eventemitter and add @output to object created
- object created.emit()
### View Encapsulation
- @Component({encapsulation:ViewEncapsulation.Emulated/None/Native})
- emulated:default
- native:uses shadow DOM,sam as emulated but only in browsers that support shadow DOM
### Local Reference
- Added to templates
- Can use only inside the template
- ```<input type="text" #localReferencename>```
- used anywhere defines the entire template
- get access to elements inside the template 
### @Viewchild() &@Contentchild()
- @ViewChild('serverContentInput', {static: true}) serverContentInput: ElementRef;
- getting access to any element directly from ts code
- like localreference
- serverContentInput.nativeElement

### ngContent
- <ng-content></ng-content>
- something you want to display between your component selector,add ng-content in that component
# ngOnInit()
- Life cycle hook
- ngOnChanges()
- ngOnInit()
- ngDoCheck()
- ngAfterContentInit()
- ngContentChecked()
- ngAfterViewInit()
- ngAfterViewChecked()
- ngOnDestroy()
- 



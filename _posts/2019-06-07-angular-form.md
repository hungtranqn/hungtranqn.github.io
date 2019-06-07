layout: post
title: Angular form Ionic 4
---

## How to use Form control on angular

### Import APIs for Reactive forms
- In App.module
```typescript
	import { ReactiveFormsModule } from '@angular/forms';

	@NgModule({
	  declarations: [...],
	  imports: [
	    ...,
	    ReactiveFormsModule
	  ],
	  providers: [...],
	  bootstrap: [...]
	})
	export class AppModule { }
```
- In page/component 
```
	@NgModule({
	  imports: [
	    CommonModule,
	    FormsModule,
	    ReactiveFormsModule,
	    IonicModule,
	    RouterModule.forChild(routes),
	    TranslateModule.forChild()
	  ],
	  declarations: [SimplewalletPage]
	})
```
### Create form in Component
```
	import { Component, OnInit } from '@angular/core';
	import { FormGroup, FormControl } from '@angular/forms';

	@Component({
	  selector: 'example',
	  templateUrl: './example.html',
	  styleUrls: ['./example.scss']
	})
	export class Example implements OnInit {
	  rfContact: FormGroup;
	  constructor() { }

	  ngOnInit() {
	    this.rfContact = new FormGroup({
	      contactName: new FormControl(),
	      email: new FormControl(),
	      social: new FormGroup({
	        facebook: new FormControl(),
	        twitter: new FormControl(),
	        website: new FormControl()
	      }),
	      tel: new FormControl()
	    });
	  }

	  onSubmit() {
	    // Do something awesome
	    console.log(this.rfContact);
	  }
	}
```
### 
# Angular Material File Input for @angular/material 19.x


## Description

An Angular Material File Input.


## DEMO

@see [DEMO stackblitz](https://stackblitz.com/edit/demo-ngx-mat-file-input)

@see [LIVE DEMO](https://github.com/developer-1-nng/angular-material-components/)

![Alt Text](demo_file_input.png)

 Choose the version corresponding to your Angular version:

 Angular     | @nng-components/angular-material-file-input
 ----------- | -------------------
 19          | 19.x+


## Getting started

```
npm install --save @nng-components/angular-material-file-input
```

## Setup

```
import { NgxMatFileInputModule } from '@nng-components/angular-material-file-input';

@NgModule({
   ...
   imports: [
        ...
        NgxMatFileInputModule
   ]
   ...
})
export class AppModule { }
```

@see [src/app/demo-fileinput/demo-fileinput.module.ts](src/app/demo-fileinput/demo-fileinput.module.ts)

## Using the component

### File Input (ngx-mat-file-input)

```
<mat-form-field>
   <ngx-mat-file-input [formControl]="fileControl" [multiple]="multiple" [accept]="accept" [color]="color">
   </ngx-mat-file-input>
</mat-form-field>
```

#### You can provide a custom icon by using the directive *ngxMatFileInputIcon*

```
<mat-form-field>
   <ngx-mat-file-input [formControl]="fileControl" [multiple]="multiple" [accept]="accept"
   [color]="color">
      <mat-icon ngxMatFileInputIcon>folder</mat-icon>
   </ngx-mat-file-input>
</mat-form-field>
```

#### You can use with all properties of MatFormField such as appearance variants, hint...

```
<mat-form-field appearance="outline">
  <ngx-mat-file-input [formControl]="file3Control">
  </ngx-mat-file-input>
  <mat-hint>Hint</mat-hint>
</mat-form-field>
```

#### List of @Input

| @Input        	| Type     	| Default value 	| Description                                                          	|
|---------------	|----------	|---------------	|----------------------------------------------------------------------	|
| **disabled**      	| boolean  	| null          	| If true, the file input is readonly.                	|
| **multiple**      	| boolean  	| false          	| If true, the file input allows the user to select more than one file.                	|
| **accept**    	   | string   | null           | Limiting accepted file types (For example: accept="image/png, image/jpeg" or accept=".png, .jpg, .jpeg" — Accept PNG or JPEG files.) 	|
| **color**      	| ThemePalette  	| null          	| Theme color palette for the component.                	|

## Theming
- @see @angular/material [Using a pre-built theme](https://material.angular.io/guide/theming#using-a-pre-built-theme)
- Add the Material Design icon font to your index.html
```
<link href="https://fonts.googleapis.com/icon?family=Material+Icons&display=block" rel="stylesheet">
```

## License
MIT
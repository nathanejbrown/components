## API Report File for "components-srcs"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { AfterViewInit } from '@angular/core';
import { ChangeDetectorRef } from '@angular/core';
import { CheckboxRequiredValidator } from '@angular/forms';
import { ControlValueAccessor } from '@angular/forms';
import { ElementRef } from '@angular/core';
import { EventEmitter } from '@angular/core';
import { FocusableOption } from '@angular/cdk/a11y';
import * as i0 from '@angular/core';
import * as i3 from '@angular/material/core';
import { InjectionToken } from '@angular/core';
import { MatRipple } from '@angular/material/core';
import { NgZone } from '@angular/core';
import { Provider } from '@angular/core';
import { ThemePalette } from '@angular/material/core';

// @public (undocumented)
export const MAT_CHECKBOX_CONTROL_VALUE_ACCESSOR: any;

// @public
export const MAT_CHECKBOX_DEFAULT_OPTIONS: InjectionToken<MatCheckboxDefaultOptions>;

// @public
export function MAT_CHECKBOX_DEFAULT_OPTIONS_FACTORY(): MatCheckboxDefaultOptions;

// @public (undocumented)
export const MAT_CHECKBOX_REQUIRED_VALIDATOR: Provider;

// @public (undocumented)
export class MatCheckbox implements AfterViewInit, ControlValueAccessor, FocusableOption {
    constructor(_elementRef: ElementRef<HTMLElement>, _changeDetectorRef: ChangeDetectorRef, _ngZone: NgZone, tabIndex: string, _animationMode?: string | undefined, _options?: MatCheckboxDefaultOptions | undefined);
    protected _animationClasses: {
        uncheckedToChecked: string;
        uncheckedToIndeterminate: string;
        checkedToUnchecked: string;
        checkedToIndeterminate: string;
        indeterminateToChecked: string;
        indeterminateToUnchecked: string;
    };
    // (undocumented)
    _animationMode?: string | undefined;
    ariaDescribedby: string;
    ariaLabel: string;
    ariaLabelledby: string | null;
    readonly change: EventEmitter<MatCheckboxChange>;
    get checked(): boolean;
    set checked(value: boolean);
    color: string | undefined;
    protected _createChangeEvent(isChecked: boolean): MatCheckboxChange;
    get disabled(): boolean;
    set disabled(value: boolean);
    disableRipple: boolean;
    // (undocumented)
    _elementRef: ElementRef<HTMLElement>;
    focus(): void;
    protected _getAnimationTargetElement(): HTMLInputElement;
    // (undocumented)
    protected _handleInputClick(): void;
    id: string;
    get indeterminate(): boolean;
    set indeterminate(value: boolean);
    readonly indeterminateChange: EventEmitter<boolean>;
    _inputElement: ElementRef<HTMLInputElement>;
    get inputId(): string;
    // (undocumented)
    _isRippleDisabled(): boolean;
    _labelElement: ElementRef<HTMLInputElement>;
    labelPosition: 'before' | 'after';
    name: string | null;
    // (undocumented)
    static ngAcceptInputType_checked: unknown;
    // (undocumented)
    static ngAcceptInputType_disabled: unknown;
    // (undocumented)
    static ngAcceptInputType_disableRipple: unknown;
    // (undocumented)
    static ngAcceptInputType_indeterminate: unknown;
    // (undocumented)
    static ngAcceptInputType_required: unknown;
    // (undocumented)
    static ngAcceptInputType_tabIndex: unknown;
    // (undocumented)
    ngAfterViewInit(): void;
    // (undocumented)
    _onBlur(): void;
    // (undocumented)
    _onInputClick(): void;
    // (undocumented)
    _onInteractionEvent(event: Event): void;
    _onLabelTextChange(): void;
    _onTouched: () => any;
    // (undocumented)
    _onTouchTargetClick(): void;
    _preventBubblingFromLabel(event: MouseEvent): void;
    // (undocumented)
    registerOnChange(fn: (value: any) => void): void;
    // (undocumented)
    registerOnTouched(fn: any): void;
    required: boolean;
    // @deprecated
    ripple: MatRipple;
    // (undocumented)
    setDisabledState(isDisabled: boolean): void;
    tabIndex: number;
    toggle(): void;
    value: string;
    // (undocumented)
    writeValue(value: any): void;
    // (undocumented)
    static ɵcmp: i0.ɵɵComponentDeclaration<MatCheckbox, "mat-checkbox", ["matCheckbox"], { "ariaLabel": { "alias": "aria-label"; "required": false; }; "ariaLabelledby": { "alias": "aria-labelledby"; "required": false; }; "ariaDescribedby": { "alias": "aria-describedby"; "required": false; }; "id": { "alias": "id"; "required": false; }; "required": { "alias": "required"; "required": false; }; "labelPosition": { "alias": "labelPosition"; "required": false; }; "name": { "alias": "name"; "required": false; }; "value": { "alias": "value"; "required": false; }; "disableRipple": { "alias": "disableRipple"; "required": false; }; "tabIndex": { "alias": "tabIndex"; "required": false; }; "color": { "alias": "color"; "required": false; }; "checked": { "alias": "checked"; "required": false; }; "disabled": { "alias": "disabled"; "required": false; }; "indeterminate": { "alias": "indeterminate"; "required": false; }; }, { "change": "change"; "indeterminateChange": "indeterminateChange"; }, never, ["*"], false, never>;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatCheckbox, [null, null, null, { attribute: "tabindex"; }, { optional: true; }, { optional: true; }]>;
}

// @public
export class MatCheckboxChange {
    checked: boolean;
    source: MatCheckbox;
}

// @public
export type MatCheckboxClickAction = 'noop' | 'check' | 'check-indeterminate' | undefined;

// @public
export interface MatCheckboxDefaultOptions {
    clickAction?: MatCheckboxClickAction;
    color?: ThemePalette;
}

// @public (undocumented)
export class MatCheckboxModule {
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatCheckboxModule, never>;
    // (undocumented)
    static ɵinj: i0.ɵɵInjectorDeclaration<MatCheckboxModule>;
    // (undocumented)
    static ɵmod: i0.ɵɵNgModuleDeclaration<MatCheckboxModule, [typeof i2.MatCheckbox], [typeof i3.MatCommonModule, typeof i3.MatRippleModule, typeof _MatCheckboxRequiredValidatorModule], [typeof i2.MatCheckbox, typeof i3.MatCommonModule, typeof _MatCheckboxRequiredValidatorModule]>;
}

// @public
export class MatCheckboxRequiredValidator extends CheckboxRequiredValidator {
    // (undocumented)
    static ɵdir: i0.ɵɵDirectiveDeclaration<MatCheckboxRequiredValidator, "mat-checkbox[required][formControlName],             mat-checkbox[required][formControl], mat-checkbox[required][ngModel]", never, {}, {}, never, never, false, never>;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatCheckboxRequiredValidator, never>;
}

// @public
export class _MatCheckboxRequiredValidatorModule {
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<_MatCheckboxRequiredValidatorModule, never>;
    // (undocumented)
    static ɵinj: i0.ɵɵInjectorDeclaration<_MatCheckboxRequiredValidatorModule>;
    // (undocumented)
    static ɵmod: i0.ɵɵNgModuleDeclaration<_MatCheckboxRequiredValidatorModule, [typeof i1.MatCheckboxRequiredValidator], never, [typeof i1.MatCheckboxRequiredValidator]>;
}

// @public
export const enum TransitionCheckState {
    Checked = 1,
    Indeterminate = 3,
    Init = 0,
    Unchecked = 2
}

// (No @packageDocumentation comment for this package)

```

## Change detection operations
- sets `ViewState.firstCheck` to true if a view is checked for the first time and to false if it was already checked before
checks and updates input properties on a child component/directive `instance`
- updates child view `change detection state` (part of change detection strategy implementation)
- `runs change detection` for the embedded views (repeats the steps in the list)
- calls `OnChanges` lifecycle hook on a child component if bindings changed
- calls `OnInit` and `ngDoCheck` on a child component (OnInit is called only during first check)
- updates `ContentChildren query list` on a child view component `instance`
- calls `AfterContentInit` and `AfterContentChecked` lifecycle hooks on child component instance (AfterContentInit is called only during first check)
- updates DOM `interpolations` for the current view if properties on current view component instance changed
- `runs change detection` for a child view (repeats the steps in this list)
- updates `ViewChildren query list` on the current view component instance
- calls `AfterViewInit` and `AfterViewChecked` lifecycle hooks on child component instance (AfterViewInit is called only during first check)
- disables checks for the current view (part of change detection strategy implementation)

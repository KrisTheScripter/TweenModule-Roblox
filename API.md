# (CUSTOM VARIABLES)

+ parameters = {
	parameter = value,
	parameter = value,
	...
}
+ Positions = {
 	Vector3
 	Vector3
 	Vector3
}
+ Property = "TweenInfo" or "WaitUntilCompleted"

# (READABLE ONLY VARIABLES)
> [!WARNING]
> Do not try to set the property by changing a variable!

+ Object - the object to tween
+ PlayingTween - the currently playing tween
+ WaitUntilCompleted - determites whenether the module should wait for tween to end or not
+ TweenInfo - current TweenInfo


# (FUNCTIONS)
> [!WARNING]
> Do not try to create errors by providing wrong arguments!

## Module:
```
.new(object - basepart or model) - returns a TweenObject
:GetTweenObjects() - returns all tweenobjects
```

## TweenObject:
```
:SetProperty(property, value) - changes given property's value to given value
:PivotTo(CFrame) - pivot object to the given CFrame
:TransferTo(Position - Vector3 or nil, Rotation - Vector3 or nil) - tweens object position and rotation
:Tween(parameters) - tweens object's given parameters
:Curve(CurveService - ModuleScript, Positions, Visualize - boolean) - tweens object using curve (quadratic interpolation), requires path to curveservice (returns tween)
:Interpolate(Instance, PropertyName, Value) - tweens object's property to given value (number or string) (if string then adds value to property's value) (returns tween)
:StopTween() - stops playing tween if it is
:Destroy() - destroys tweenobject
```

<!---
custom_mark
@startuml
namespace Ui #EEEEEE{
	 Class View
	 Class VisualEfl
	 Class VisualText
	 Class VisualMask
	 Class _ViewRootVisual
	 Class _ViewImpl
	 Class _VisualEflImpl
	 Interface IViewTouchEventListener
	 Interface IViewActionEventListener
	 
	 Vi.Base.Object<|-- View 
	 Vi.Animations.Visual<|--VisualEfl
	 Vi.Animations.Visual <|-- VisualMask
	 View *-- _ViewImpl
	 _ViewImpl o--IViewTouchEventListener
	 _ViewImpl o--IViewActionEventListener
	 VisualEfl *-- _VisualEflImpl
	 _VisualEflImpl -->Vi.Base.Color
	 _VisualEflImpl -->Vi.Base.FloatPoint
	 _VisualEflImpl -->Vi.Base.FloatDimension
	 VisualEfl<|--VisualText
	 VisualEfl<|--_ViewRootVisual 
 }
@enduml
custom_mark
-->

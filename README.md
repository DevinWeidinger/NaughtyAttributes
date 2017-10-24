# NaughtyAttributes
Attribute Extensions for Unity

## System Requirements
Unity 2017.1.0 or later versions. Feel free to try older version

## Drawer Attributes
Provide special draw options to serialized fields.
A field can have only one DrawerAttribute. If a field has more than one, only the bottom one will be used.

### Slider
The same as Unity's **Range** attribute.
There is no difference between the two, you can use whatever you like, I just wanted to support a custom slider attribute.

![code](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/Slider_Code.PNG)

![inspector](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/Slider_Inspector.PNG)

### MinMaxSlider
A double slider. The **min value** is saved to the **X** property, and the **max value** is saved to the **Y** property of a **Vector2** field.

![code](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/MinMaxSlider_Code.PNG)

![inspector](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/MinMaxSlider_Inspector.PNG)

### ReorderableList
Provides array type fields with an interface for easy reordering of elements.

![code](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/ReorderableList_Code.PNG)

![inspector](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/ReorderableList_Inspector.gif)

### Button
A method can be marked as a button. A button appears in the inspector and executes the method if clicked.
Works both with instance and static methods.

![code](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/Button_Code.PNG)

![inspector](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/Button_Inspector.PNG)

### Dropdown
Provides an interface for dropdown value selection.

![code](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/Dropdown_Code.PNG)

![inspector](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/Dropdown_Inspector.gif)

### ResizableTextArea
A resizable text area where you can see the whole text.
Unlike Unity's **Multiline** and **TextArea** attributes where you can see only 3 rows of a given text, and in order to see it or modify it you have to manually scroll down to the desired row.

![code](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/ResizableTextArea_Code.PNG)

![inspector](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/ResizableTextArea_Inspector.gif)

### ShowNonSerializedField
Shows non-serialized fields in the inspector.
All non-serialized fields are displayed at the botton of the inspector before the method buttons.
Keep in mind that if you change a non-static, non-serialized field in the code - the value in the inspector will be updated after you press **Play** in the editor.
There is non such issue with static non-serialized fields because their values are updated at compile time.

![code](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/ShowNonSerializedField_Code.PNG)

![inspector](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/ShowNonSerializedField_Inspector.PNG)

## DrawCondition Attributes
Can be used to specify when a given serialized field is visible, and when not. A field can have only one DrawConditionAttribute.

### ShowIf / HideIf
![code](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/ShowIf_Code.PNG)

![inspector](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/ShowIf_Inspector.gif)

## Group Attributes
Serialized fields can be grouped in different groups.
A field can have only one GroupAttribute.

### BoxGroup
Surrounds grouped fields with a box.

![code](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/BoxGroup_Code.PNG)

![inspector](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/BoxGroup_Inspector.PNG)

## Validator Attributes
Used for validating the fields. A field can have infinite number of validator attributes.

### MinValue / MaxValue
Clamps integer and float fields.

![code](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/MinValueMaxValue_Code.PNG)

![inspector](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/MinValueMaxValue_Inspector.gif)

### Required
Used to remind the developer that a given reference type field is required.

![code](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/Required_Code.PNG)

![inspector](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/Required_Inspector.PNG)

### ValidateInput
The most powerful ValidatorAttribute.

![code](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/ValidateInput_Code.PNG)

![inspector](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/ValidateInput_Inspector.PNG)

## Meta Attributes
Give the fields meta data. A field can have infinite number of meta attributes.

### Section
Can be used for grouping fields. The same as Unity's **Header** attribute.
There is no difference between the two, you can use whatever you like, I just wanted to support a custom header attribute.

![code](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/Section_Code.PNG)

![inspector](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/Section_Inspector.PNG)

### BlankSpace
The same as Unity's **Space** attribute.
There is no difference between the two, you can use whatever you like, I just wanted to support a custom space attribute.

![code](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/BlankSpace_Code.PNG)

![inspector](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/BlankSpace_Inspector.PNG)

### InfoBox
Used for providing additional information.

![code](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/InfoBox_Code.PNG)

![inspector](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/InfoBox_Inspector.PNG)

### OnValueChanged
Detects a value change and executes a callback.

![code](https://github.com/dbrizov/NaughtyAttributes/blob/master/Assets/Plugins/NaughtyAttributes/Documentation/OnValueChanged_Code.PNG)

## License
MIT License

Copyright (c) 2017 Denis Rizov

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

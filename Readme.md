# Qlik Date Picker Widget

This is a very simple QlikSense Widget that allows you to pick a data and store it in a variable. It uses 2 lines of HTML code and HTML5 date picker capabilities so there is no JS library to render a calendar. 

If you are afraid to use extensions which could break, this is a great way to add date picker functionality as it uses Qlik's built-in Leonardo UI and actions which should work with any new version without breaking. 

[Download Widget](https://github.com/NickAkincilar/QlikDatePickerWidget/blob/master/QlikNavigationWidgets.zip?raw=true)

**Here is the entire code of this widget:**


    <label class="lui-label">{{settings.varLabel}}</label><input type="date" class="lui-input lui-input-group__item " style="width:140px;" ng-model="selectVal" ng-init="opt=settings.selVarValue" ng-change="app.variable.setContent(settings.selVarName, (selectVal.getMonth() + 1) + '/' + selectVal.getDate() + '/' + selectVal.getFullYear());">
    

![enter image description here](https://github.com/NickAkincilar/QlikDatePickerWidget/blob/master/DatePicker.png?raw=true)
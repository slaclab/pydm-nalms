# pydm-nalms

This project contains PyDM widgets and datasource for the NALMS alarm system.


The datasource is in a draft phase, likely to be reformatted once the extension points have been configured for PyDM datasources. Alternatively, the datasource script could be added directly to pydm in 'pydm/data_plugins/`.


The Alarm Tree qill have to be registered in `pydm/widgets/qtplugins.py` by adding the line entry:

```python
PyDMAlarmTreePlugin = qtplugin_factory(PyDMAlarmTree,
                                         group=WidgetCategory.DISPLAY,
                                         extensions=[AlarmTreeEditorExtension])

```
音量ボタンの使用タイミングは意外と少ないものです。ボタンにマクロを登録して片手操作や作業を効率化しましょう。


仕様  
アンドロイド端末の物理ボタンからマクロを実行するためのスクリプトです。物理ボタンの組み合わせで最大16個のマクロやアプリを実行できます。
動作にはローカル変数を用いています。音量ボタンの入力は up→(u) down→(d) として変数に追加され,長押しは大文字として入力されます。一定時間待機後,変数に応じたアプリやマクロを実行出来ます。このスクリプトを導入すると音量ボタンでの音量操作が不可能になります。代わりにDownボタンを長押しすることでポップアップを呼び出し,そこから変更します。また,ポップアップと同時に音量が瞬時に0になるので,素早く操作したい際にも比較的問題にはなりません。


  
初期状態での仕様  
  
u   Spotify起動  
uu  ライトルーム起動  
uuu ギャラリー起動  

d   ドロワー表示  
dd  翻訳アプリ  
ddd Duolingo  

ud  通知領域の表示 ON・OFF  

U   Notion起動  
Uu  画面の回転 有効無効の切り替え  
Uuu 録音開始  

D   音量レベル0 & 音量ポップアップ表示  
Dd  音量ポップアップ表示 (音量レベル変更無し)  
Ddd スクリーンショット  


導入方法  
MacroDroidから.macroのファイルをインポートしてください。

カスタム方法  

if文で現在の変数を検知する箇所が数カ所あります。その中の命令を自身の使用したいマクロに変更してご使用ください。(導入してから変更するのがやりやすいと思います) またご自身の操作速度や端末にあわせて待機時間を変更するとより快適に使用できます。1回から3回連続入力のそれぞれに待機時間を設定できます。条件を追加することで更に設定できるマクロの数を増やすことも可能です。(du Ud Du などは未設定のため)







{
	"globalVariables": [],
	"macro": {
		"aiGenerated": 0,
		"breakpoints": [],
		"disabledTimestamp": 0,
		"exportedActionBlocks": [],
		"forceEvenIfNotEnabledTimestamp": 0,
		"isActionBlock": false,
		"isExtra": false,
		"isFavourite": true,
		"lastEditedTimestamp": 1779814106454,
		"localVariables": [
			{
				"description": "",
				"dictionary": {
					"entries": [],
					"isArray": false,
					"variableType": 4,
					"type": "Dictionary"
				},
				"isActionBlockWorkingVar": true,
				"isLocalVar": true,
				"isSecure": false,
				"m_booleanValue": false,
				"m_decimalValue": 0,
				"m_intValue": 0,
				"m_name": "ボタンオブザーバー",
				"m_stringValue": "",
				"m_type": 2,
				"supportsInput": false,
				"supportsOutput": true
			}
		],
		"localVarsAlphabetical": true,
		"m_GUID": -7511375742914767000,
		"m_actionList": [
			{
				"childrenCollapsed": false,
				"dontLogIfConditionIsFalse": false,
				"disableLogging": false,
				"m_SIGUID": -8396142902443998000,
				"m_classType": "IfConditionAction",
				"m_comment": "",
				"m_constraintList": [
					{
						"m_not": false,
						"m_siGuidThatInvoked": -8156981931340199000,
						"m_triggerName": "音量UPボタン押した時: 音量を変えず現状維持",
						"disableLogging": false,
						"m_SIGUID": -5427501971954793000,
						"m_classType": "TriggerThatInvokedConstraint",
						"m_comment": "",
						"m_constraintList": [],
						"m_isDisabled": false,
						"m_isOrCondition": false
					}
				],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"booleanDictionaryKeys": {
					"keys": []
				},
				"dictionaryKeys": [],
				"dictionaryOrArrayType": -1,
				"existingManualKeyType": 0,
				"m_booleanInvert": false,
				"m_darkMode": -1,
				"m_doubleRandomMax": 0,
				"m_doubleRandomMin": 0,
				"m_falseLabel": "False",
				"m_intExpression": false,
				"m_intRandom": false,
				"m_intRandomMax": 0,
				"m_intRandomMin": 0,
				"m_intValueDecrement": false,
				"m_intValueIncrement": false,
				"m_newBooleanValue": false,
				"m_newDoubleValue": 0,
				"m_newIntValue": 0,
				"m_newStringValue": "[lv=ボタンオブザーバー]u",
				"m_trueLabel": "True",
				"m_userPrompt": false,
				"m_userPromptEmptyAtStart": false,
				"m_userPromptPassword": false,
				"m_userPromptShowCancel": true,
				"m_userPromptStopAfterCancel": true,
				"m_variable": {
					"description": "",
					"dictionary": {
						"entries": [],
						"isArray": false,
						"variableType": 4,
						"type": "Dictionary"
					},
					"isActionBlockWorkingVar": true,
					"isLocalVar": true,
					"isSecure": false,
					"m_booleanValue": false,
					"m_decimalValue": 0,
					"m_intValue": 0,
					"m_name": "ボタンオブザーバー",
					"m_stringValue": "",
					"m_type": 2,
					"supportsInput": false,
					"supportsOutput": true
				},
				"disableLogging": false,
				"m_SIGUID": -6887062379844102000,
				"m_classType": "SetVariableAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"disableLogging": false,
				"m_SIGUID": -5512225028161431000,
				"m_classType": "EndIfAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"childrenCollapsed": false,
				"dontLogIfConditionIsFalse": false,
				"disableLogging": false,
				"m_SIGUID": -7858874344089654000,
				"m_classType": "IfConditionAction",
				"m_comment": "",
				"m_constraintList": [
					{
						"m_not": false,
						"m_siGuidThatInvoked": -7463864198728226000,
						"m_triggerName": "音量DOWNボタン押した時: 音量を変えず現状維持",
						"disableLogging": false,
						"m_SIGUID": -5534338912950224000,
						"m_classType": "TriggerThatInvokedConstraint",
						"m_comment": "",
						"m_constraintList": [],
						"m_isDisabled": false,
						"m_isOrCondition": false
					}
				],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"booleanDictionaryKeys": {
					"keys": []
				},
				"dictionaryKeys": [],
				"dictionaryOrArrayType": -1,
				"existingManualKeyType": 0,
				"m_booleanInvert": false,
				"m_darkMode": -1,
				"m_doubleRandomMax": 0,
				"m_doubleRandomMin": 0,
				"m_falseLabel": "False",
				"m_intExpression": false,
				"m_intRandom": false,
				"m_intRandomMax": 0,
				"m_intRandomMin": 0,
				"m_intValueDecrement": false,
				"m_intValueIncrement": false,
				"m_newBooleanValue": false,
				"m_newDoubleValue": 0,
				"m_newIntValue": 0,
				"m_newStringValue": "[lv=ボタンオブザーバー]d",
				"m_trueLabel": "True",
				"m_userPrompt": false,
				"m_userPromptEmptyAtStart": false,
				"m_userPromptPassword": false,
				"m_userPromptShowCancel": true,
				"m_userPromptStopAfterCancel": true,
				"m_variable": {
					"description": "",
					"dictionary": {
						"entries": [],
						"isArray": false,
						"variableType": 4,
						"type": "Dictionary"
					},
					"isActionBlockWorkingVar": true,
					"isLocalVar": true,
					"isSecure": false,
					"m_booleanValue": false,
					"m_decimalValue": 0,
					"m_intValue": 0,
					"m_name": "ボタンオブザーバー",
					"m_stringValue": "",
					"m_type": 2,
					"supportsInput": false,
					"supportsOutput": true
				},
				"disableLogging": false,
				"m_SIGUID": -6390102632360048000,
				"m_classType": "SetVariableAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"disableLogging": false,
				"m_SIGUID": -7426764345101056000,
				"m_classType": "EndIfAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"childrenCollapsed": false,
				"dontLogIfConditionIsFalse": false,
				"disableLogging": false,
				"m_SIGUID": -6734293543987673000,
				"m_classType": "IfConditionAction",
				"m_comment": "",
				"m_constraintList": [
					{
						"m_not": false,
						"m_siGuidThatInvoked": -7935720922104640000,
						"m_triggerName": "音量UPボタン押した時 (長押し): 音量を変えず現状維持",
						"disableLogging": false,
						"m_SIGUID": -7437496105969726000,
						"m_classType": "TriggerThatInvokedConstraint",
						"m_comment": "",
						"m_constraintList": [],
						"m_isDisabled": false,
						"m_isOrCondition": false
					}
				],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"booleanDictionaryKeys": {
					"keys": []
				},
				"dictionaryKeys": [],
				"dictionaryOrArrayType": -1,
				"existingManualKeyType": 0,
				"m_booleanInvert": false,
				"m_darkMode": -1,
				"m_doubleRandomMax": 0,
				"m_doubleRandomMin": 0,
				"m_falseLabel": "False",
				"m_intExpression": false,
				"m_intRandom": false,
				"m_intRandomMax": 0,
				"m_intRandomMin": 0,
				"m_intValueDecrement": false,
				"m_intValueIncrement": false,
				"m_newBooleanValue": false,
				"m_newDoubleValue": 0,
				"m_newIntValue": 0,
				"m_newStringValue": "[lv=ボタンオブザーバー]U",
				"m_trueLabel": "True",
				"m_userPrompt": false,
				"m_userPromptEmptyAtStart": false,
				"m_userPromptPassword": false,
				"m_userPromptShowCancel": true,
				"m_userPromptStopAfterCancel": true,
				"m_variable": {
					"description": "",
					"dictionary": {
						"entries": [],
						"isArray": false,
						"variableType": 4,
						"type": "Dictionary"
					},
					"isActionBlockWorkingVar": true,
					"isLocalVar": true,
					"isSecure": false,
					"m_booleanValue": false,
					"m_decimalValue": 0,
					"m_intValue": 0,
					"m_name": "ボタンオブザーバー",
					"m_stringValue": "",
					"m_type": 2,
					"supportsInput": false,
					"supportsOutput": true
				},
				"disableLogging": false,
				"m_SIGUID": -5228496270598362000,
				"m_classType": "SetVariableAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"disableLogging": false,
				"m_SIGUID": -6949973214645776000,
				"m_classType": "EndIfAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"childrenCollapsed": false,
				"dontLogIfConditionIsFalse": false,
				"disableLogging": false,
				"m_SIGUID": -6878513443922100000,
				"m_classType": "IfConditionAction",
				"m_comment": "",
				"m_constraintList": [
					{
						"m_not": false,
						"m_siGuidThatInvoked": -5785325525166320000,
						"m_triggerName": "音量DOWNボタン押した時 (長押し): 音量を変えず現状維持",
						"disableLogging": false,
						"m_SIGUID": -5355375230216474000,
						"m_classType": "TriggerThatInvokedConstraint",
						"m_comment": "",
						"m_constraintList": [],
						"m_isDisabled": false,
						"m_isOrCondition": false
					}
				],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"booleanDictionaryKeys": {
					"keys": []
				},
				"dictionaryKeys": [],
				"dictionaryOrArrayType": -1,
				"existingManualKeyType": 0,
				"m_booleanInvert": false,
				"m_darkMode": -1,
				"m_doubleRandomMax": 0,
				"m_doubleRandomMin": 0,
				"m_falseLabel": "False",
				"m_intExpression": false,
				"m_intRandom": false,
				"m_intRandomMax": 0,
				"m_intRandomMin": 0,
				"m_intValueDecrement": false,
				"m_intValueIncrement": false,
				"m_newBooleanValue": false,
				"m_newDoubleValue": 0,
				"m_newIntValue": 0,
				"m_newStringValue": "[lv=ボタンオブザーバー]D",
				"m_trueLabel": "True",
				"m_userPrompt": false,
				"m_userPromptEmptyAtStart": false,
				"m_userPromptPassword": false,
				"m_userPromptShowCancel": true,
				"m_userPromptStopAfterCancel": true,
				"m_variable": {
					"description": "",
					"dictionary": {
						"entries": [],
						"isArray": false,
						"variableType": 4,
						"type": "Dictionary"
					},
					"isActionBlockWorkingVar": true,
					"isLocalVar": true,
					"isSecure": false,
					"m_booleanValue": false,
					"m_decimalValue": 0,
					"m_intValue": 0,
					"m_name": "ボタンオブザーバー",
					"m_stringValue": "",
					"m_type": 2,
					"supportsInput": false,
					"supportsOutput": true
				},
				"disableLogging": false,
				"m_SIGUID": -7973428965661670000,
				"m_classType": "SetVariableAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"disableLogging": false,
				"m_SIGUID": -8363621412736827000,
				"m_classType": "EndIfAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"color": -1,
				"separatorLabel": "",
				"disableLogging": false,
				"m_SIGUID": -8841885136774631000,
				"m_classType": "SeparatorAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"childrenCollapsed": false,
				"dontLogIfConditionIsFalse": false,
				"disableLogging": false,
				"m_SIGUID": -6641059172721037000,
				"m_classType": "IfConditionAction",
				"m_constraintList": [
					{
						"comparisonType": 0,
						"enableRegex": false,
						"ignoreCase": true,
						"type": 1,
						"value1": "{strlen=ボタンオブザーバー}",
						"value2": "1",
						"disableLogging": false,
						"m_SIGUID": -8758073522445800000,
						"m_classType": "CompareValueConstraint",
						"m_constraintList": [],
						"m_isDisabled": false,
						"m_isOrCondition": false
					}
				],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"m_delayInMilliSeconds": 250,
				"m_delayInSeconds": 0,
				"m_useAlarm": true,
				"unitForVariables": 0,
				"disableLogging": false,
				"m_SIGUID": -4647567932941393000,
				"m_classType": "PauseAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"childrenCollapsed": false,
				"dontLogIfConditionIsFalse": false,
				"disableLogging": false,
				"m_SIGUID": -6996638219878095000,
				"m_classType": "IfConditionAction",
				"m_constraintList": [
					{
						"comparisonType": 0,
						"enableRegex": false,
						"ignoreCase": true,
						"type": 1,
						"value1": "{strlen=ボタンオブザーバー}",
						"value2": "１",
						"disableLogging": false,
						"m_SIGUID": -6027250003814425000,
						"m_classType": "CompareValueConstraint",
						"m_constraintList": [],
						"m_isDisabled": false,
						"m_isOrCondition": false
					}
				],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"childrenCollapsed": true,
				"dontLogIfConditionIsFalse": false,
				"disableLogging": false,
				"m_SIGUID": -5130678536578036000,
				"m_classType": "IfConditionAction",
				"m_comment": "",
				"m_constraintList": [
					{
						"comparisonType": 0,
						"enableRegex": false,
						"ignoreCase": false,
						"type": 2,
						"value1": "{lv=ボタンオブザーバー}",
						"value2": "u",
						"disableLogging": false,
						"m_SIGUID": -7812596843692978000,
						"m_classType": "CompareValueConstraint",
						"m_comment": "",
						"m_constraintList": [],
						"m_isDisabled": false,
						"m_isOrCondition": false
					}
				],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"m_applicationName": "Spotify",
				"m_excludeFromRecents": false,
				"m_packageToLaunch": "com.spotify.music",
				"m_startNew": false,
				"option": 0,
				"disableLogging": false,
				"m_SIGUID": -7398907347937307000,
				"m_classType": "LaunchActivityAction",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"disableLogging": false,
				"m_SIGUID": -5807013227947937000,
				"m_classType": "EndIfAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"childrenCollapsed": true,
				"dontLogIfConditionIsFalse": false,
				"disableLogging": false,
				"m_SIGUID": -6110484319525792000,
				"m_classType": "IfConditionAction",
				"m_comment": "",
				"m_constraintList": [
					{
						"comparisonType": 0,
						"enableRegex": false,
						"ignoreCase": false,
						"type": 2,
						"value1": "{lv=ボタンオブザーバー}",
						"value2": "d",
						"disableLogging": false,
						"m_SIGUID": -8024123535688203000,
						"m_classType": "CompareValueConstraint",
						"m_comment": "",
						"m_constraintList": [],
						"m_isDisabled": false,
						"m_isOrCondition": false
					}
				],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"childrenCollapsed": false,
				"dontLogIfConditionIsFalse": false,
				"disableLogging": false,
				"m_SIGUID": -9086091068326886000,
				"m_classType": "IfConditionAction",
				"m_comment": "",
				"m_constraintList": [
					{
						"drawerType": 0,
						"option": 1,
						"disableLogging": false,
						"m_SIGUID": -8469580092837917000,
						"m_classType": "DrawerStateConstraint",
						"m_comment": "",
						"m_constraintList": [],
						"m_isDisabled": false,
						"m_isOrCondition": false
					}
				],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"drawerType": 0,
				"m_option": 0,
				"swipeAreaColour": -7829368,
				"swipeAreaHeight": 45,
				"swipeAreaOpacity": 50,
				"swipeAreaOption": 0,
				"swipeAreaVerticalOffset": 50,
				"swipeAreaVisibleWidth": 10,
				"swipeAreaWidth": 10,
				"disableLogging": false,
				"m_SIGUID": -5658969538572187000,
				"m_classType": "MacroDroidDrawerAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"m_applicationName": "翻訳",
				"m_excludeFromRecents": false,
				"m_packageToLaunch": "com.google.android.apps.translate",
				"m_startNew": false,
				"option": 0,
				"disableLogging": false,
				"m_SIGUID": -5119670216707248000,
				"m_classType": "LaunchActivityAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": true,
				"m_isOrCondition": false
			},
			{
				"dontLogIfConditionIsFalse": false,
				"disableLogging": false,
				"m_SIGUID": -9185506221833951000,
				"m_classType": "ElseAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"drawerType": 0,
				"m_option": 1,
				"swipeAreaColour": -7829368,
				"swipeAreaHeight": 45,
				"swipeAreaOpacity": 50,
				"swipeAreaOption": 0,
				"swipeAreaVerticalOffset": 50,
				"swipeAreaVisibleWidth": 10,
				"swipeAreaWidth": 10,
				"disableLogging": false,
				"m_SIGUID": -7906821518122991000,
				"m_classType": "MacroDroidDrawerAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"disableLogging": false,
				"m_SIGUID": -6304938956006187000,
				"m_classType": "EndIfAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"disableLogging": false,
				"m_SIGUID": -6749938639299341000,
				"m_classType": "EndIfAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"childrenCollapsed": false,
				"dontLogIfConditionIsFalse": false,
				"disableLogging": false,
				"m_SIGUID": -5488631302614121000,
				"m_classType": "IfConditionAction",
				"m_comment": "",
				"m_constraintList": [
					{
						"comparisonType": 0,
						"enableRegex": false,
						"ignoreCase": false,
						"type": 2,
						"value1": "{lv=ボタンオブザーバー}",
						"value2": "D",
						"disableLogging": false,
						"m_SIGUID": -8591802600109745000,
						"m_classType": "CompareValueConstraint",
						"m_comment": "",
						"m_constraintList": [],
						"m_isDisabled": false,
						"m_isOrCondition": false
					}
				],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"m_forceVibrateOff": false,
				"m_streamIndexArray": [
					false,
					true,
					false,
					false,
					false,
					false,
					false,
					false
				],
				"m_streamVolumeArray": [
					0,
					0,
					0,
					0,
					0,
					0,
					0,
					0
				],
				"m_variables": [
					null,
					null,
					null,
					null,
					null,
					null,
					null,
					null
				],
				"m_volume": -1,
				"setInForeground": false,
				"varDictionaryKeys": [
					null,
					null,
					null,
					null,
					null,
					null,
					null,
					null
				],
				"disableLogging": false,
				"m_SIGUID": -8468241674547233000,
				"m_classType": "SetVolumeAction",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"audioStream": 1,
				"disableLogging": false,
				"m_SIGUID": -6482428899441379000,
				"m_classType": "ShowVolumePopupAction",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"disableLogging": false,
				"m_SIGUID": -7026337556697967000,
				"m_classType": "EndIfAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"variableNames": [
					"ボタンオブザーバー"
				],
				"disableLogging": false,
				"m_SIGUID": -5838785393277150000,
				"m_classType": "ClearVariablesAction",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"disableLogging": false,
				"m_SIGUID": -6455359592951545000,
				"m_classType": "EndIfAction",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"disableLogging": false,
				"m_SIGUID": -5588686491865728000,
				"m_classType": "EndIfAction",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"color": -1,
				"separatorLabel": "",
				"disableLogging": false,
				"m_SIGUID": -8965300873393702000,
				"m_classType": "SeparatorAction",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"childrenCollapsed": false,
				"dontLogIfConditionIsFalse": false,
				"disableLogging": false,
				"m_SIGUID": -8711077514152229000,
				"m_classType": "IfConditionAction",
				"m_constraintList": [
					{
						"comparisonType": 0,
						"enableRegex": false,
						"ignoreCase": true,
						"type": 1,
						"value1": "{strlen=ボタンオブザーバー}",
						"value2": "2",
						"disableLogging": false,
						"m_SIGUID": -7325796336508763000,
						"m_classType": "CompareValueConstraint",
						"m_constraintList": [],
						"m_isDisabled": false,
						"m_isOrCondition": false
					}
				],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"m_delayInMilliSeconds": 350,
				"m_delayInSeconds": 0,
				"m_useAlarm": true,
				"unitForVariables": 0,
				"disableLogging": false,
				"m_SIGUID": -5505491975307263000,
				"m_classType": "PauseAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"childrenCollapsed": false,
				"dontLogIfConditionIsFalse": false,
				"disableLogging": false,
				"m_SIGUID": -7806564910215559000,
				"m_classType": "IfConditionAction",
				"m_constraintList": [
					{
						"comparisonType": 0,
						"enableRegex": false,
						"ignoreCase": true,
						"type": 1,
						"value1": "{strlen=ボタンオブザーバー}",
						"value2": "2",
						"disableLogging": false,
						"m_SIGUID": -8460839383574857000,
						"m_classType": "CompareValueConstraint",
						"m_constraintList": [],
						"m_isDisabled": false,
						"m_isOrCondition": false
					}
				],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"childrenCollapsed": false,
				"dontLogIfConditionIsFalse": false,
				"disableLogging": false,
				"m_SIGUID": -6978010445327963000,
				"m_classType": "IfConditionAction",
				"m_comment": "",
				"m_constraintList": [
					{
						"comparisonType": 0,
						"enableRegex": false,
						"ignoreCase": false,
						"type": 2,
						"value1": "{lv=ボタンオブザーバー}",
						"value2": "uu",
						"disableLogging": false,
						"m_SIGUID": -8304429615104624000,
						"m_classType": "CompareValueConstraint",
						"m_comment": "",
						"m_constraintList": [],
						"m_isDisabled": false,
						"m_isOrCondition": false
					}
				],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"m_applicationName": "Lightroom",
				"m_excludeFromRecents": false,
				"m_packageToLaunch": "com.adobe.lrmobile",
				"m_startNew": false,
				"option": 0,
				"disableLogging": false,
				"m_SIGUID": -4844079998204845000,
				"m_classType": "LaunchActivityAction",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"disableLogging": false,
				"m_SIGUID": -7951075000872676000,
				"m_classType": "EndIfAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"childrenCollapsed": false,
				"dontLogIfConditionIsFalse": false,
				"disableLogging": false,
				"m_SIGUID": -6094381523052245000,
				"m_classType": "IfConditionAction",
				"m_comment": "",
				"m_constraintList": [
					{
						"comparisonType": 0,
						"enableRegex": false,
						"ignoreCase": false,
						"type": 2,
						"value1": "{lv=ボタンオブザーバー}",
						"value2": "dd",
						"disableLogging": false,
						"m_SIGUID": -5867637983312541000,
						"m_classType": "CompareValueConstraint",
						"m_comment": "",
						"m_constraintList": [],
						"m_isDisabled": false,
						"m_isOrCondition": false
					}
				],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"m_applicationName": "翻訳",
				"m_excludeFromRecents": false,
				"m_packageToLaunch": "com.google.android.apps.translate",
				"m_startNew": false,
				"option": 0,
				"disableLogging": false,
				"m_SIGUID": -6210261892806366000,
				"m_classType": "LaunchActivityAction",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"disableLogging": false,
				"m_SIGUID": -8514671291191043000,
				"m_classType": "EndIfAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"variableNames": [
					"ボタンオブザーバー"
				],
				"disableLogging": false,
				"m_SIGUID": -8907417584269433000,
				"m_classType": "ClearVariablesAction",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"disableLogging": false,
				"m_SIGUID": -6082673799913832000,
				"m_classType": "EndIfAction",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"disableLogging": false,
				"m_SIGUID": -5699457171437123000,
				"m_classType": "EndIfAction",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"color": -1,
				"separatorLabel": "",
				"disableLogging": false,
				"m_SIGUID": -6313171674612543000,
				"m_classType": "SeparatorAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"childrenCollapsed": false,
				"dontLogIfConditionIsFalse": false,
				"disableLogging": false,
				"m_SIGUID": -5161475057122452000,
				"m_classType": "IfConditionAction",
				"m_constraintList": [
					{
						"comparisonType": 0,
						"enableRegex": false,
						"ignoreCase": true,
						"type": 1,
						"value1": "{strlen=ボタンオブザーバー}",
						"value2": "3",
						"disableLogging": false,
						"m_SIGUID": -7942110359655689000,
						"m_classType": "CompareValueConstraint",
						"m_constraintList": [],
						"m_isDisabled": false,
						"m_isOrCondition": false
					}
				],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"m_delayInMilliSeconds": 20,
				"m_delayInSeconds": 0,
				"m_useAlarm": true,
				"unitForVariables": 0,
				"disableLogging": false,
				"m_SIGUID": -6785774090502669000,
				"m_classType": "PauseAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"childrenCollapsed": false,
				"dontLogIfConditionIsFalse": false,
				"disableLogging": false,
				"m_SIGUID": -6937897962756197000,
				"m_classType": "IfConditionAction",
				"m_constraintList": [
					{
						"comparisonType": 0,
						"enableRegex": false,
						"ignoreCase": true,
						"type": 1,
						"value1": "{strlen=ボタンオブザーバー}",
						"value2": "3",
						"disableLogging": false,
						"m_SIGUID": -9064579506205614000,
						"m_classType": "CompareValueConstraint",
						"m_constraintList": [],
						"m_isDisabled": false,
						"m_isOrCondition": false
					}
				],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"childrenCollapsed": false,
				"dontLogIfConditionIsFalse": false,
				"disableLogging": false,
				"m_SIGUID": -6743622555491378000,
				"m_classType": "IfConditionAction",
				"m_comment": "",
				"m_constraintList": [
					{
						"comparisonType": 0,
						"enableRegex": false,
						"ignoreCase": false,
						"type": 2,
						"value1": "{lv=ボタンオブザーバー}",
						"value2": "uuu",
						"disableLogging": false,
						"m_SIGUID": -5438490220542135000,
						"m_classType": "CompareValueConstraint",
						"m_comment": "",
						"m_constraintList": [],
						"m_isDisabled": false,
						"m_isOrCondition": false
					}
				],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"m_applicationName": "ギャラリー",
				"m_excludeFromRecents": false,
				"m_packageToLaunch": "com.sec.android.gallery3d",
				"m_startNew": false,
				"option": 0,
				"disableLogging": false,
				"m_SIGUID": -5321778538130980000,
				"m_classType": "LaunchActivityAction",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"disableLogging": false,
				"m_SIGUID": -7901253502366960000,
				"m_classType": "EndIfAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"childrenCollapsed": false,
				"dontLogIfConditionIsFalse": false,
				"disableLogging": false,
				"m_SIGUID": -8261335432371080000,
				"m_classType": "IfConditionAction",
				"m_comment": "",
				"m_constraintList": [
					{
						"comparisonType": 0,
						"enableRegex": false,
						"ignoreCase": false,
						"type": 2,
						"value1": "{lv=ボタンオブザーバー}",
						"value2": "ddd",
						"disableLogging": false,
						"m_SIGUID": -6346217262235654000,
						"m_classType": "CompareValueConstraint",
						"m_comment": "",
						"m_constraintList": [],
						"m_isDisabled": false,
						"m_isOrCondition": false
					}
				],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"m_applicationName": "Duolingo",
				"m_excludeFromRecents": false,
				"m_packageToLaunch": "com.duolingo",
				"m_startNew": false,
				"option": 0,
				"disableLogging": false,
				"m_SIGUID": -7999363179612223000,
				"m_classType": "LaunchActivityAction",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"disableLogging": false,
				"m_SIGUID": -8810417760463519000,
				"m_classType": "EndIfAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"variableNames": [
					"ボタンオブザーバー"
				],
				"disableLogging": false,
				"m_SIGUID": -5139148358867538000,
				"m_classType": "ClearVariablesAction",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"disableLogging": false,
				"m_SIGUID": -7480702760279355000,
				"m_classType": "EndIfAction",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"disableLogging": false,
				"m_SIGUID": -5493756305565645000,
				"m_classType": "EndIfAction",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"color": -1,
				"separatorLabel": "",
				"disableLogging": false,
				"m_SIGUID": -8113804915778627000,
				"m_classType": "SeparatorAction",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			}
		],
		"m_category": "音量新規用",
		"m_constraintList": [],
		"m_description": "",
		"m_descriptionOpen": false,
		"m_enabled": true,
		"m_excludeLog": false,
		"m_headingColor": 0,
		"m_isOrCondition": false,
		"m_name": "音量完全版 改訂版",
		"m_triggerList": [
			{
				"m_dontChangeVolume": true,
				"m_monitorOption": 0,
				"m_notConfigured": false,
				"m_option": 0,
				"disableLogging": false,
				"m_SIGUID": -8156981931340199000,
				"m_classType": "VolumeButtonTrigger",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"m_dontChangeVolume": true,
				"m_monitorOption": 0,
				"m_notConfigured": false,
				"m_option": 1,
				"disableLogging": false,
				"m_SIGUID": -7463864198728226000,
				"m_classType": "VolumeButtonTrigger",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"m_dontChangeVolume": true,
				"m_monitorOption": 0,
				"m_notConfigured": false,
				"m_option": 2,
				"disableLogging": false,
				"m_SIGUID": -7935720922104640000,
				"m_classType": "VolumeButtonTrigger",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			},
			{
				"m_dontChangeVolume": true,
				"m_monitorOption": 0,
				"m_notConfigured": false,
				"m_option": 3,
				"disableLogging": false,
				"m_SIGUID": -5785325525166320000,
				"m_classType": "VolumeButtonTrigger",
				"m_comment": "",
				"m_constraintList": [],
				"m_isDisabled": false,
				"m_isOrCondition": false
			}
		]
	},
	"macroExportVersion": 1
}

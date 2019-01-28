If you want to style the tree-style-tabs to look like below use the High Contrast Theme and add the follwoing css to the custom overwrite

```
/* Show title of unread tabs with red and italic font */
/*
.tab.unread .label {
  color: red !important;
  font-style: italic !important;
}
*/

/* Add private browsing indicator per tab */
.tab.private-browsing .label:before {
  content: "🕶";
}


.tab {
background-color: #F2F2F2;
margin: 1px;
border-bottom: 1px solid #A3A3A3;
}
.tab .label {
color: black;
margin-left: 10px !important;
}

.newtab-button-box {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  height: 30px;
}
.newtab-button {
background-color: #D3D3D3 !important;
padding: 5px !important;

}

:root.simulate-svg-context-fill .newtab-button::before {
  background: black;
}
#tabbar {
  top: 30px !important;
  bottom: 0 !important;
  background-color: #D3D3D3;
}
.tab.pinned {
  margin-top: 30px;
}

.closebox::after {
  content: "⨉";
  background: none;
  line-height: 1;
  mask: none;
  text-align: center;
  width: 1.5em;
}

.tab.active {
  background-color: #2F343F;
}
.tab.active .label {
  font-weight: bold;
  font-size: 14px;
}
.tab.active .twisty,
.tab.active .label,
.tab.active .counter {
  color: #FFFFFF;
}
```

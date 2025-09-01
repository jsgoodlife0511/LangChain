### (1) partial_variable (partial variable filling)  
A common use case is when you want to consistently include certain variables. A typical example is date or time.  
def get_today(): <-- example  
&nbsp;&nbsp;return datetime.now().strftime("%B %d")  
PromptTemplate( ...  
&nbsp;&nbsp;partial_variables={  
&nbsp;&nbsp;&nbsp;&nbsp;"today": get_today  # pass partial variable as a form of dictionary  
&nbsp;&nbsp;},   
&nbsp;&nbsp;... )  
### (2) MessagePlaceHolder
A reserved spot for messages that will be filled in later.  


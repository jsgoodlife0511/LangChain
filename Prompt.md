### (1) partial_variable (partial variable filling)  
def get_today(): <-- example  
    return datetime.now().strftime("%B %d")  
PromptTemplate( ...  
    partial_variables={  
        "today": get_today  # pass partial variable as a form of dictionary  
    },   
    ... )  
### (2)  


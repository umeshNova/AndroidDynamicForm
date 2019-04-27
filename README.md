# AndroidDynamicForm

# It's main purpose to load form dynamically from server. This library will work as render engine to below schema



##Json Format

{
  form_title : "title",
  form_title_color : "#000",
  lang : "en"
  sections : [
               { 
                section_title : "",
                section_title_color : "",
                section_title_size : "",
                section_bacground_color : "",
                elements : [
                              {
                                type : int(ENUM) ,
                                enabled : bool,
                                id : long,
                                label : "",
                                cache : bool,
                                default_value : ["",""], //1.default_val, 2 :hint
                                error_text : "",
                                text_size : [], //1.value,2.hint
                                text_color : [], //1.value,2.hint
                                options : [""], // in case of spinner or radio
                                validations : [""] // enums //need discussion
                              }
                             ]
               }    
              ]

}

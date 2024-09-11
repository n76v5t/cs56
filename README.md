java c
Analyzing large data sets with the R package 
Objective: to acquire skills in statistical data processing and graphics using the R   programming language.
Objectives: to get acquainted with the interface   and   functionality   of   R,   to   learn   how   to   process, analyze, and visualize various types of   data using the R package.
Methodological recommendations 
1. Familiarize yourself with the R program andRStudio. R is a programming language for statistical   processing, data analysis, and graphics, as well as a free   and open-source computing environment as part of   the GNU project. R supports a wide range of   statistical   and numerical methods and powerful additional functional and analytical      capabilities   (built-in package   library).   Packages   are   libraries   for   specific   functions   or   special   applications. R   comes with   a   basic   set   of   packages. As of   2019, there are more than   12,000 packages available.
R   is   widely   used   in   the   social   sciences,   statistics,   economics,   insurance,   sociology,   finance,   physics, etc.
R is available for all operating systems,   including Linux,   Mac   OS,   and   Windows.
R   is   a   matrix,   object-oriented programming language. This   means that,   in   theory,   anything   can   be   saved   as   an R object. Each   object has its own   class that   describes what   this   object   contains   and   what   each   function   can   do   with   this   data.   For   example,   plot(x) produces   one   result   if x   is   a   regression   and   another   if   it   is   a   vector.
The R package can be downloaded and installed absolutely free   of   charge.   To   do   this, visit      the CRAN website (https://cran.r-project.org) and download the installation   package. After running it,   you need to   select the appropriate installation   parameters (language,   package components, and other
settings). After the program starts, a dialog   box opens - the console window, where all commands and   the results of   their execution are displayed (Fig.   165).
Figure   165. The dialog box (console) for starting the R package To make it   easier   for the user to   work   with   the   R   package,   an   interface program called RStudio   was   created. Note   that   working   with   R   and   RStudio   is   almost identical. For   example, RStudio   provides   many convenient tools,   and   it has   a pleasant   and   more understandable   interface.   To   download   it,   you   must first install the R   package and then download the   corresponding file:
https://www.rstudio.com/products /rstudio/download   /#download.
After launching the program, a window consisting of   4 blocks will open (Fig.   166).   The   RStudio   environment   consists   of   windows:
1)    script   (for writing   code   and preparing   it   for launch);
2)    console (displays all   commands   and the results   of   their execution);
3)    Workspace (Environment) - to   display   all   objects   and   their   descriptions.   The History tab shows the history   of   commands   entered   by   the   user;
4)    Files (displays the working directory - folder), Plots (for visualizing all charts), Packages (shows   all   installed   library   packages), Help (for   reference   information).
Figure   166. The RStudio startup dialog box For example, using the R package   as   a regular   calculator,   we   can   write   certain   mathematical   actions   in   the   script   window   and   press   the Run button   or   use   the Cntr + Enter button   combination   (Figure   167).
Figure   167. Performing simple calculations in RStudio 
After   executing   the   code,   the   calculation   result   appeared   in   the   console   window,   and   the   History tab simultaneously displayed all the commands that the user entered.
All functions are entered   accordingly.If   you   don't   know   what   kind   of   function   you   are   working   with, you   should   call   up   the   help.   To   do this,   in the   script. window,   enter   a   question   mark before   the   function   name   and   click   the Run button.   All   the   necessary   reference   information   will   be   displayed   in   the Help window   (tab)   (Figure   168).
Figure   168. Launching help in RStudio The   user   can    create   variables.    To    do    this,    enter   the   variable    designation    in    the    console   window, then the   assignment   sign   (<-) and the value to which it corresponds. For example, y = 100 (Fig. 169).Figure   169. Creating a variable in RStudio 
The Environment window   displays   the   result   of   creating   the   variable.   You   can   also   perform. calculations (y*2) and create expressions (x   = y^2)   (Figure   170).
Figure   170. Simple calculations in RStudio 
In R, any command is a function   that   can be passed   as   an   argument.   Functions can be easily combined.
The assignment symbol is   "<-". You can also use the wildcard "=". That is, the following two expressions are equivalent:
>   а <- 2; >   а   =   2.
Arguments are given in parentheses.
Usually, it is better to use quotation marks for names, but it   is not   always   necessary.
"#" is used for   comments.
Commands are separated by a semicolon   ";"   or   a   carriage return character. If   you want to place   more than one expression on one line, you must use the   ";" separator.
R   is   case   sensitive:   "a"   and   "A"   are   two   different   objects,   so   all   functions   and   arguments   must be entered in lowercase.Traditionally, the underscore character   "_"   is not used   in names.   In   most   cases,   it   is   better   to   use   the   dot   character   ".".   Avoid   using   the   underscore   character   as   the   first   character   in   an   object   name.
There are special   characters   in R:   NA: Not Available;
NaN: Not a Number, for example, uncertainty 0/0; Inf: Infinity;   -Inf: (Minus infinity).
You can exit R using q (). The no argument means that the session is not to be saved.
The R package works with the following data types: logical, integer, real,   complex,   character, and   list.
The analytical capabilities of   the R package are due to the ability   to work with   various   objects,   in particular:
1.      Vectors   are the most basic   of   R   objects,   and   can   contain   only   one type   of   data. You   can   create a vector   by using   the c () function, which combines several elements of   the same type. You can   also   create   a   sequence   using   the:   symbol   or   the seq () function.   For   example,    1:5    creates    a   vector   sequence of   numbers from   1 to 5. The seq () function allows   you   to specify   the   interval   between numbers.   You   can   repeat   the   pattern   using   the rep    () function.   You   can   also   create   a   numeric   vector   with   missing values by using the numeric () function,   or   a   character vector with character () or a logical   vector with logical ().
2.      Factors   are   similar to   vectors, but   with   a   defined   set   of levels. Factor represents   a   nominal   or   rank   scale.   It   is   used   to   represent   Y   in   classification   models,   and   the factor () f代 写Analyzing large data sets with the R packageMatlab
代做程序编程语言unction   transforms   a   vector   into a   factor.   Also, factor   can be sorted   using   the   option   ordered   = T or the function ordered ().
3.      Matrices are similar to vectors, but with specific instructions for output. A matrix is   a   two-   dimensional set of   elements of   the same type   (table).   If   you want   to   create   a   matrix,   one   way   is   to   use   the matrix () function. You   enter a vector, a   set ofrows or   columns,   and   you   can   tell   R   how   to   interpret   the data (by default, as   columns).The cbind () and rbind () functions   combine   vectors   in   a   matrix   by   column   or   by   row.   The   dimension   of   the matrix   can be   obtained using the dim () function.   Otherwise,   the nrow () and ncol () functions   return   the   number   of   rows   and   columns, respectively.
4.      Arrays   are   similar   to   matrices,   but   can   have   more   than   two   dimensions.   An   array   is   a   multidimensional set of   elements of   the same type. Array.
must   be   symmetrical   in   all   dimensions.   The   vector   objects   that   make up   t h   e   array   must be   of the   same type, but not necessarily of   numeric type.
5.      A list is a vector for R objects. Lists area collection   of   R   objects.   The list () function   creates   a list; unlist () transforms a list into   a vector. Mostly,   it   is   convenient   to   store   in   the   form   of   lists   either   some data of   the same type that      corresponds to different iterations, for example, many models, or to store   heterogeneous   data that have   a   semantic   connection,   for   example,   different   statistical   characteristics   of   a   single   model.
6. A   dataframe   is   similar   to   a   matrix,   but   does   not   require   all   columns   to   be   identical   in   type.   The   structure   is   a   list   of variables/vectors   of the    same   length. Data.frame -   a   two-dimensional   data   set   (table).   Unlike   matrices,   columns   in   a   data.frame   can   contain   data   of different   types.   However,   there   can   be   only   one   data   type   within   each   column.   This   is   because   a data.frame is   a   list   of vectors   (columns). Therefore, different functions can   be applied to thedata.frame. 
7.      Formulas area special form. of   expressing relationships between variables in an equation. Formulas      are    used    when      building      models       to       determine      the      functional      relationship      between   parameters. The dot symbol   "(.)" replaces all available variables.
8.      Classes   is   a   data type   for a variable,   and   a variable of   this   type   is   an   object   -   an   instance   of   the class). Classes are attached to objects as attributes. All   objects   in   R   have   their   own   class,   type,   and dimension.All   objects   support   naming   the   elements   they   contain.   To   do   this,   use   the   character    "   or   ''.   Similarly   to   vectors,   matrices   and   data.frames   have   such   properties   as rownames and colnames, which   allow   you   to   change   the   names   of   columns   and   rows.
To delete names, you can assign a   special   type NULL.
Converting data types is done through a group of   functions   that   are based   on as.
Indexing in R is an effective and powerful tool for working with   data.   Indexes can be numeric, boolean, and textual.
Three types of   expressions are   used for indexing:   [ - selects   elements of   a vector/list/array, etc;
$ - selects one element   from the   data.frame/list by   its name;
[[- selects elements from a vector/list/array, etc. but   discards names   if   they   exist.The   indexing   features   allow   you   to   change   the   position   of items   and   duplicate   them.   To   delete   elements   by index value, a minus sign is added   before them. To   add   a new   element   (column/row   in the   data.frame) to   the   list, anew   name   or   numeric   index   is   used.
If   an index is accessed that does not exist, the   special value NA is returned.
2. Working in RStudio: graphical features. Before you   start working   in   RStudio, you need   to   import   data.   To   enter   data,   in   addition   to   the   manual mode, you can use the   Environment window, the Inport Dataset button, and   specify what type of   file   to import and where   from. Weremind you that the filename must be in English and consist   of   one   word (Fig. 171).Figure   171. Importing data into RStudio 
The result is a data table containing information about   the   age   and   salary   of   the   bank's customers (Figure   172).
Figure   172. Input data for analysis in RStudio 
If   you   want   to   name   the   columns   or   change   them, goto   the   Untitled*1 script   window   and run the command:
colnames(Salary)<-c('Age_years','Wage_th_UAH').
As a result, we get new names for the table columns (Figure   173).
Figure   173. Changing the names of table columns in RStudio The R package   (RStudio) has   a powerful visualization unit. To work with   graphics   in R,   you need    to    install    the    appropriate    package    -    ggplot2,    that    is,    run    the install.packages ("ggplot2") command or select the Graphics package in the library and click   the Install button.
In ggplot2, any   type   of   infographic   is   the   result   of   the   interaction   of   a   number   of   elements:
1)      of   the data array;
2)    schemes of   correspondence of   variables to the array of   visual means (aesthetic);
3)      geometric object (geom);
4)      statistical transformation (stat);
5)      coordinate system (coord);
6)      guide;
7)      panels (facet);
8)      artistic design (theme).
Visualize   the original information space. To do this, use the command:   plot(Salary$Age_years,Salary$Wage_th_UAH) (Fig.   174).
Figure   174. Building a chart in RStudio The    user    can    also    change    the    parameters    of   the    dot      diagram:      select    the    type,      color,       and   thickness.                                                    To                                                    do                                                    this,                                                       run                                                    the                                                    command:   plot(Salary$Age_years,Salary$Wage_th_UAH,col='red',lwd=2) (Fig.   175).
Figure   175. Editing a graph in RStudio 
To change the axis labels and name the dot   plot, run   the   following   command:   plot(Salary$Age_years,Salary$Wage_th_UAH,col='red',lwd
=2,xlab = 'Age_of_Bank_Customers',ylab = 'Salary_thousand_hryvnias',main   = 'Dependence_of_income_on_age') (Fig.   176).
Figure   176. Finished visualization in RStudio 
The user   can   also   change the type   of chart. For   example, let's   turn   a   dot   chart   into   a bar   chart.   To do this, you need to change the geometric object to   aes(xlab = 'Age of bank customers' 
= cyl)) + geom_bar()+ coord_polar().
So, the source data has been downloaded and visualized.

         
加QQ：99515681  WX：codinghelp

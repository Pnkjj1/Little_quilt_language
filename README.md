# Little_quilt_language
 ‘Little   Quilt’,   Language   of   Expressions:   is   small   enough   to permit   a   short   description,   different   enough   to   require   description,   yet   representative enough    of    programming    languages    to    make    description    worthwhile.    The    earliest programming  languages  began  with  integers,  reals  and  arrays  of  integers  and  reals;  these too   can   be   visualized   and   discussed   independently   of   the   constructs   in   the   language. Likewise Little Quilt manipulates geometric objects with a height, a width and texture.Little Quilt Project:I  came  across  this  project  as  an  assignment  given  by  Prof.  Uday  Khedker  from  I.I.T.  Bombay.  As  we  approached  him  to  acquire  a  BE  project  under  his  guidance,  he  wanted  to  test  our  programming  skills  on  the  basis  of  this  mini  project.  He  told  us  that  in  order   to   develop   an   interpreter   we   would   need   to   learn Lex   and   Yacc   compiler generation  tools  in  Linux,  which  we  knew  nothing  about.  But  we  decided  to  take  the  challenge  and  we  could  finish  it  in  a  short  span  of  13  days.  We  got  final  year  project  on the basis of successful accomplishment of this mini project. I  led  entire  coding  work.  I  got  good  experience  of  developing  a  lexer  and  parser  of  a  high  level  language.  Development  of  interpretation  logic  of  program  was  also  a  great fun. This  really  prompted  my  interest  in  compilers.  We  discovered  unique  solutions  to  the problems we faced. Some of them are listed below.• Computer representation/evaluation of user defined multi-parameter functions. • Computer representation/evaluation of list of parameters in a user defined   functions. • Ingenious use of stack to make behave a global variable like a local variable    during unwinding of inherent recursion of Yacc parser. Since  ‘Little  Quilt’  is  a  high  level  language,  its  grammar  is  as  complex  as  that  of  any typical high-level language. Hence coding the grammar in Yacc was another challenge. An example of a program in Little Quilt.let  fun unturn(x) = turn(turn(turn(x))) fun pile(x,y) = unturn(sew(turn(y),turn(x))) val aa = pile(a,turn(turn(a))) val bb = pile(unturn(b),turn(b)) val p = sew(bb,aa) val q = sew(aa,bb) in pile(p,q) end









Install Lex and Yacc tools.
Run this "lqp" file by command ./lqp -d

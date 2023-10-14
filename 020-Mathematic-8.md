---
title: 020-Mathematic-8
date: 2023-03-22 13:49:01
tags:
categories: [Mathematic]
toc: true
---

本次笔记相关教材为同济第七版高等数学上册以及习题全解指南两本书

# 附录中的积分表

## （一）、含有$ax+b$的积分

1. $\int{\frac{dx}{ax+b}}=\frac1a\ln|ax+b|+C$
<br/><br/>

2. $\int{(ax+b)}^\mu dx=\frac1{a(\mu+1)}(ax+b)^{\mu+1}+C(\mu\neq-1)$
<br/><br/>

3. $\int\frac x{ax+b}dx=\frac1{a^2}(ax+b-b\ln|ax+b|)+C$
<br/><br/>

4. $\int\frac{x^2}{ax+b}dx=\frac1{a^3}[\frac12(ax+b)^2-2b(ax+b)+b^2\ln|ax+b|]+C$
<br/><br/>

5. $\int\frac{dx}{x(ax+b)}=-\frac1b\ln|\frac{ax+b}x|+C$
<br/><br/>

6. $\int\frac{dx}{x^2(ax+b)}=-\frac1{bx}+\frac a{b^2}\ln|\frac{ax+b}x|+C$
<br/><br/>

7. $\int\frac{x}{(ax+b)^2}dx=\frac1{a^2}(\ln|ax+b|+\frac b{ax+b})+C$
<br/><br/>

8. $\int\frac{x^2}{(ax+b)^2}dx=\frac1{a^3}(ax+b-2b\ln|ax+b|-\frac{b^2}{ax+b})+C$
<br/><br/>

9. $\int\frac{dx}{x(ax+b)^2}=\frac1{b(ax+b)}-\frac1{b^2}\ln|\frac{ax+b}x|+C$
<br/><br/>

## 含有$\sqrt{ax+b}$的积分

10. $\int\sqrt{ax+b}\:dx=\frac2{3a}\sqrt{(ax+b)^3}+C$
<br/><br/>

11. $\int x\sqrt{ax+b}\;dx=\frac{2}{15a^2}(3ax-2b)\sqrt{(ax+b)^3}+C$
<br/><br/>

12. $\int x^2\sqrt{ax+b}\,dx=\frac2{105a^3}(15a^2x^2-12abx+8b^2)\sqrt{(ax+b)^3}+C$
<br/><br/>

13. $\int\frac x{\sqrt{ax+b}}\;dx=\frac2{3a^2}(ax-2b)\sqrt{ax+b}+C$
<br/><br/>

14. $\int\frac{x^2}{\sqrt{ax+b}}\;dx=\frac2{15a^3}(3a^2x^2-4abx+8b^2)\sqrt{ax+b}+C$
<br/><br/>

15. $\int\frac{dx}{x\sqrt{ax+b}}=\begin{cases}\frac1{\sqrt b}\ln|\frac{\sqrt{ax+b}-\sqrt{b}}{\sqrt{ax+b}+\sqrt{b}}|+C(b>0) \\\\ \frac2{\sqrt{-b}}\arctan\sqrt{\frac{ax+b}{-b}}+C(b< 0) \end{cases}$
<br/><br/>

16. $\int\frac{dx}{x^2\sqrt{ax+b}}=-\frac{\sqrt{ax+b}}{bx}-\frac a{2b}\int\frac{dx}{x\sqrt{ax+b}}$
<br/><br/>

17. $\int\frac{\sqrt{ax+b}}x\;dx=2\sqrt{ax+b}+b\int\frac{dx}{x\sqrt{ax+b}}$
<br/><br/>

18. $\int\frac{\sqrt{ax+b}}{x^2}\;dx=-\frac{\sqrt{ax+b}}{x}+\frac a2\int\frac{dx}{x\sqrt{ax+b}}$
<br/><br/>

## （三）含有$x^2\pm a^2$的积分

19. $\int\frac{dx}{x^2+a^2}=\frac1a\arctan\frac xa+C$
<br/><br/>

20. $\int\frac{dx}{(x^2+a^2)^n}=\frac x{2(n-1)a^2(x^2+a^2)^{n-1}}+\frac{2n-3}{2(n-1)a^2}\int\frac{dx}{(x^2+a^2)^{n-1}}$
<br/><br/>

21. $\int\frac{dx}{x^2-a^2}=\frac1{2a}\ln|\frac{x-a}{x+a}|+C$
<br/><br/>

## （四）、含有$ax^2+b(a>0)$的积分

22. $\int\frac{dx}{ax^2+b}=\begin{cases}\frac1{\sqrt{ab}}\arctan\sqrt{\frac ab}x+C(b>0)\\\\\frac1{2\sqrt{-ab}}\ln|\frac{\sqrt a\;x-\sqrt{-b}}{\sqrt a\,x+\sqrt{-b}}|+C(b<0) \end{cases}$
<br/><br/>

23. $\int\frac x{ax^2+b}\,dx=\frac1{2a}\ln|ax^2+b|+C$
<br/><br/>

24. $\int\frac{x^2}{ax^2+b}\,dx=\frac xa-\frac ba\int\frac{dx}{ax^2+b}$
<br/><br/>

25. $\int\frac{dx}{x(ax^2+b)}=\frac1{2b}\ln\frac{x^2}{|ax^2+b|}+C$
<br/><br/>

26. $\int\frac{dx}{x^2(ax^2+b)}=-\frac1{bx}-\frac ab\int\frac{dx}{ax^2+b}$
<br/><br/>

27. $\int\frac{dx}{x^3(ax^2+b)}=\frac a{2b^2}\ln\frac{|ax^2+b|}{x^2}-\frac1{2bx^2}+C$
<br/><br/>

28. $\int\frac{dx}{(ax^2+b)^2}=\frac x{2b(ax^2+b)}+\frac1{2b}\int\frac{dx}{ax^2+b}$
<br/><br/>

## （五）、含有$ax^2+bx+c(a>0)$的积分

29. $\int\frac{dx}{ax^2+bx+c}=\begin{cases}\frac2{\sqrt{4ac-b^2}}\arctan\frac{2ax+b}{\sqrt{4ac-b^2}}+C(b^2<4ac)\\\\\frac1{\sqrt{b^2-4ac}}\ln|\frac{2ax+b-\sqrt{b^2-4ac}}{2ax+b+\sqrt{b^2-4ac}}|+C(b^2>4ac)\end{cases}$
<br/><br/>

30. $\int\frac x{ax^2+bx+c}\,dx=\frac1{2a}\ln|ax^2+bx+c|-\frac b{2a}\int\frac{dx}{ax^2+bx+c}$
<br/><br/>

## （六）、含有$\sqrt{x^2+a^2}(a>0)$的积分

31. $\int\frac{dx}{\sqrt{x^2+a^2}}=arsh\frac xa+C_1=\ln(x+\sqrt{x^2+a^2})+C$
<br/><br/>

32. $\int\frac{dx}{\sqrt{(x^2+a^2)^3}}=\frac{x}{a^2\sqrt{x^2+a^2}}+C$
<br/><br/>

33. $\int\frac{x}{\sqrt{x^2+a^2}}dx=\sqrt{x^2+a^2}+C$
<br/><br/>

34. $\int\frac{x}{\sqrt{(x^2+a^2)^3}}dx=-\frac1{\sqrt{x^2+a^2}}+C$
<br/><br/>

35. $\int\frac{x^2}{\sqrt{x^2+a^2}}dx=\frac x2\sqrt{x^2+a^2}-\frac{a^2}2\ln(x+\sqrt{x^2+a^2})+C$
<br/><br/>

36. $\int\frac{x^2}{\sqrt{(x^2+a^2)^3}}dx=-\frac x{\sqrt{x^2+a^2}}+\ln(x+\sqrt{x^2+a^2})+C$
<br/><br/>

37. $\int\frac{dx}{x\sqrt{x^2+a^2}}=\frac1a\ln\frac{\sqrt{x^2+a^2}-a}{|x|}+C$
<br/><br/>

38. $\int\frac{dx}{x^2\sqrt{x^2+a^2}}=-\frac{\sqrt{x^2+a^2}}{a^2x}+C$
<br/><br/>

39. $\int\sqrt{x^2+a^2}\,dx=\frac x2\sqrt{x^2+a^2}+\frac{a^2}2\ln(x+\sqrt{x^2+a^2})+C$
<br/><br/>

40. $\int\sqrt{(x^2+a^2)^3}\,dx=\frac x8(2x^2+5a^2)\sqrt{x^2+a^2}+\frac38a^4\ln(x+\sqrt{x^2+a^2})+C$
<br/><br/>

41. $\int x\sqrt{x^2+a^2}dx=\frac13\sqrt{(x^2+a^2)^3}+C$
<br/><br/>

42. $\int x^2\sqrt{x^2+a^2}\,dx=\frac x8(2x^2+a^2)\sqrt{x^2+a^2}-\frac{a^4}8\ln(x+\sqrt{x^2+a^2})+C$
<br/><br/>

43. $\int \frac{\sqrt{x^2+a^2}}{x}dx=\sqrt{x^2+a^2}+a\ln\frac{\sqrt{x^2+a^2}-a}{|x|}+C$
<br/><br/>

44. $\int\frac{\sqrt{x^2+a^2}}{x^2}dx=-\frac{\sqrt{x^2+a^2}}x+\ln(x+\sqrt{x^2+a^2})+C$
<br/><br/>

## （七）、含有$\sqrt{x^2-a^2}(a>0)$的积分

45. $\int\frac{dx}{\sqrt{x^2-a^2}}=\frac{x}{|x|}arch\frac{|x|}{a}+C_1=\ln|x+\sqrt{x^2-a^2}|+C$
<br/><br/>

46. $\int\frac{dx}{\sqrt{(x^2-a^2)^3}}=-\frac x{a^2\sqrt{x^2-a^2}}+C$
<br/><br/>

47. $\int\frac{x}{\sqrt{x^2-a^2}}dx=\sqrt{x^2-a^2}+C$
<br/><br/>

48. $\int\frac{x}{\sqrt{(x^2-a^2)^3}}dx=-\frac1{\sqrt{x^2-a^2}}+C$
<br/><br/>

49. $\int\frac{x^2}{\sqrt{x^2-a^2}}dx=\frac x2\sqrt{x^2-a^2}+\frac {a^2}2\ln|x+\sqrt{x^2-a^2}|+C$
<br/><br/>

50. $\int\frac{x^2}{\sqrt{(x^2-a^2)^3}}dx=-\frac x{\sqrt{x^2-a^2}}+\ln|x+\sqrt{x^2-a^2}|+C$
<br/><br/>

51. $\int\frac{dx}{x\sqrt{x^2-a^2}}=\frac 1a\arccos\frac a{|x|}+C$
<br/><br/>

52. $\int\frac{dx}{x^2\sqrt{x^2-a^2}}=\frac{\sqrt{x^2-a^2}}{a^2x}+C$
<br/><br/>

53. $\int\sqrt{x^2-a^2}\,dx=\frac x2\sqrt{x^2-a^2}-\frac{a^2}2\ln|x+\sqrt{x^2-a^2}|+C$
<br/><br/>

54. $\int\sqrt{(x^2-a^2)^3}\,dx=\frac x8(2x^2-5a^2)\sqrt{x^2-a^2}+\frac38a^4\ln|x+\sqrt{x^2-a^2}|+C$
<br/><br/>

55. $\int x\sqrt{x^2-a^2}\,dx=\frac 13\sqrt{(x^2-a^2)^3}+C$
<br/><br/>

56. $\int x^2\sqrt{x^2-a^2}\,dx=\frac x8(2x^2-a^2)\sqrt{x^2-a^2}-\frac{a^4}8\ln|x+\sqrt{x^2-a^2}|+C$
<br/><br/>

57. $\int\frac{\sqrt{x^2-a^2}}{x}dx=\sqrt{x^2-a^2}-a\arccos\frac a{|x|}+C$
<br/><br/>

58. $\int\frac{\sqrt{x^2-a^2}}{x^2}dx=-\frac{\sqrt{x^2-a^2}}{x}+\ln|x+\sqrt{x^2-a^2}|+C$
<br/><br/>

## （八）、含有$\sqrt{a^2-x^2}$的积分

59. $\int\frac{dx}{\sqrt{a^2-x^2}}=\arcsin\frac xa+C$
<br/><br/>

60. $\int\frac{dx}{\sqrt{(a^2-x^2)^3}}=\frac{x}{a^2\sqrt{a^2-x^2}}+C$
<br/><br/>

61. $\int\frac{x}{\sqrt{a^2-x^2}}dx=-\sqrt{a^2-x^2}+C$
<br/><br/>

62. $\int\frac{x}{\sqrt{(a^2-x^2)^3}}dx=\frac1{\sqrt{a^2-x^2}}+C$
<br/><br/>

63. $\int\frac{x^2}{\sqrt{a^2-x^2}}dx=-\frac x2\sqrt{a^2-x^2}+\frac{a^2}2\arcsin\frac xa+C$
<br/><br/>

64. $\int\frac{x^2}{\sqrt{(a^2-x^2)^3}}dx=\frac{x}{\sqrt{a^2-x^2}}-\arcsin\frac xa+C$
<br/><br/>

65. $\int\frac{dx}{x\sqrt{a^2-x^2}}=\frac1a\ln\frac{a-\sqrt{a^2-x^2}}{|x|}+C$
<br/><br/>

66. $\int\frac{dx}{x^2\sqrt{a^2-x^2}}=-\frac{\sqrt{a^2-x^2}}{a^2x}+C$
<br/><br/>

67. $\int\sqrt{a^2-x^2}\,dx=\frac x2\sqrt{a^2-x^2}+\frac{a^2}{2}\arcsin\frac xa+C$
<br/><br/>

68. $\sqrt{(a^2-x^2)^3}\,dx=\frac x8(5a^2-2x^2)\sqrt{a^2-x^2}+\frac38a^4\arcsin\frac xa+C$
<br/><br/>

69. $\int x\sqrt{a^2-x^2}\,dx=-\frac 13\sqrt{(a^2-x^2)^3}+C$
<br/><br/>

70. $\int x^2\sqrt{a^2-x^2}\,dx=\frac x8(2x^2-a^2)\sqrt{a^2-x^2}+\frac{a^4}8\arcsin\frac xa+C$
<br/><br/>

71. $\int\frac{\sqrt{a^2-x^2}}{x}dx=\sqrt{a^2-x^2}+a\ln\frac{a-\sqrt{a^2-x^2}}{|x|}+C$
<br/><br/>

72. $\int\frac{\sqrt{a^2-x^2}}{x^2}dx=-\frac{\sqrt{a^2-x^2}}x-\arcsin\frac xa+C$
<br/><br/>

## （九）、含有$\sqrt{\pm ax^2+bx+c}(a>0)$的积分

73. $\int\frac{dx}{\sqrt{ax^2+bx+c}}=\frac1{\sqrt a}\ln|2ax+b+2\sqrt a\sqrt{ax^2+bx+c}|+C$
<br/><br/>

74. $\int\sqrt{ax^2+bx+c}\,dx=\frac{2ax+b}{4a}\sqrt{ax^2+bx+c}+\frac{4ac-b^2}{8\sqrt{a^3}}\ln|2ax+b+2\sqrt a\sqrt{ax^2+bx+c}|+C$
<br/><br/>

75. $\int\frac x{\sqrt{ax^2+bx+c}}dx=\frac1a\sqrt{ax^2+bx+c}-\frac b{2\sqrt{a^3}}\ln|2ax+b+2\sqrt a\sqrt{ax^2+bx+c}|+C$
<br/><br/>

76. $\int\frac{dx}{\sqrt{c+bx-ax^2}}=\frac1{\sqrt{a}}\arcsin\frac{2ax-b}{\sqrt{b^2+4ac}}+C$
<br/><br/>

77. $\int\sqrt{c+bx-ax^2}\,dx=\frac{2ax-b}{4a}\sqrt{c+bx-ax^2}+\frac{b^2+4ac}{8\sqrt{a^3}}\arcsin\frac{2ax-b}{\sqrt{b^2+4ac}}+C$
<br/><br/>

78. $\int\frac{x}{\sqrt{c+bx-ax^2}}dx=-\frac1a\sqrt{c+bx-ax^2}+\frac b{2\sqrt{a^3}}\arcsin\frac{2ax-b}{\sqrt{b^2+4ac}}+C$
<br/><br/>

## （十）、含有$\sqrt{\pm\frac{x-a}{x-b}}$或$\sqrt{(x-a)(b-x)}$的积分

79. $\int\sqrt{\frac{x-a}{x-b}}dx=(x-b)\sqrt{\frac{x-a}{x-b}}+(b-a)\ln(\sqrt{|x-a|}+\sqrt{|x-b|})+C$
<br/><br/>

80. $\int\sqrt{\frac{x-a}{b-x}}dx=(x-b)\sqrt{\frac{x-a}{b-x}}+(b-a)\arcsin\sqrt{\frac{x-a}{b-a}}+C$
<br/><br/>

81. $\int\frac{dx}{\sqrt{(x-a)(b-x)}}=2\arcsin\sqrt{\frac{x-a}{b-a}}+C$ (a< b)
<br/><br/>

82. $\int\sqrt{(x-a)(b-x)}dx=\frac{2x-a-b}4\sqrt{(x-a)(b-x)}+\frac{(b-a)^2}{4}\arcsin\sqrt{\frac{x-a}{b-a}}+C$(a< b)
<br/><br/>

## （十一）、含有三角函数的积分

83. $\int\sin xdx=-\cos x+ C$
<br/><br/>

84. $\int\cos xdx=\sin x+C$
<br/><br/>

85. $\int\tan xdx=-\ln|\cos x|+C$
<br/><br/>

86. $\int\cot xdx=\ln|\sin x|+C$
<br/><br/>

87. $\int\sec xdx=\ln|\tan(\frac\pi4+\frac x2)|+C=\ln|\sec x+\tan x|+C$
<br/><br/>

88. $\int\csc xdx=\ln|\tan\frac x2|+C=\ln|\csc x-\cot x|+C$
<br/><br/>

89. $\int\sec^2xdx=\tan x+C$
<br/><br/>

90. $\int\csc^2xdx=-\cot x+C$
<br/><br/>

91. $\int\sec x\tan xdx=\sec x+C$
<br/><br/>

92. $\int\csc x\cot xdx=-\csc x+C$
<br/><br/>

93. $\int\sin^2xdx=\frac x2-\frac14\sin2x+C$
<br/><br/>

94. $\int\cos^2xdx=\frac x2+\frac14\sin2x+C$
<br/><br/>

95. $\int\sin^nxdx=-\frac1n\sin^{n-1}x\cos x+\frac{n-1}n\int\sin^{n-2}xdx$
<br/><br/>

96. $\int\cos^nxdx=\frac1n\cos^{n-1}x\sin x+\frac{n-1}n\int\cos^{n-2}xdx$
<br/><br/>

97. $\int\frac{dx}{\sin^nx}=-\frac1{n-1}\cdot\frac{\cos x}{\sin^{n-1}x}+\frac{n-2}{n-1}\int\frac{dx}{\sin^{n-2}x}$
<br/><br/>

98. $\int\frac{dx}{\cos^nx}=\frac1{n-1}\cdot\frac{\sin x}{\cos^{n-1}x}+\frac{n-2}{n-1}\int\frac{dx}{\cos^{n-2}x}$
<br/><br/>

99. $\int\cos^mx\sin^nxdx=\frac1{m+n}\cos^{m-1}x\sin^{n+1}x\frac{m-1}{m+n}\int\cos^{m-2}x\sin^nxdx$

或者
$=-\frac1{m+n}\cos^{m+1}x\sin^{n-1}x+\frac{n-1}{m+n}\int\cos^mx\sin^{n-2}xdx$
<br/><br/>

100. $\int\sin ax\cos bxdx=-\frac1{2(a+b)}\cos(a+b)x-\frac1{2(a-b)}\cos(a-b)x+C$
<br/><br/>

101. $\int\sin ax\sin bxdx=-\frac1{2(a+b)}\sin(a+b)x+\frac1{2(a-b)}\sin(a-b)x+C$
<br/><br/>

102. $\int\cos ax\cos bxdx=\frac1{2(a+b)}\sin(a+b)x+\frac1{2(a-b)}\sin(a-b)x+C$ 
<br/><br/>

103. $\int\frac{dx}{a+b\sin x}=\frac{2}{\sqrt{a^2-b^2}}\arctan\frac{a\tan\frac x2+b}{\sqrt{a^2-b^2}}+C(a^2>b^2)$
<br/><br/>

104. $\int\frac{dx}{a+b\sin x}=\frac1{\sqrt{b^2-a^2}}\ln|\frac{a\tan\frac x2+b-\sqrt{b^2-a^2}}{a\tan\frac x2+b+\sqrt{b^2-a^2}}|+C$ $(a^2< b^2)$
<br/><br/>

105. $\int\frac{dx}{a+b\cos x}=\frac2{a+b}\sqrt{\frac{a+b}{a-b}}\arctan(\sqrt{\frac{a-b}{a+b}}\tan\frac x2)+C$ $(a^2$> $b^2)$
<br/><br/>

106. $\int\frac{dx}{a+b\cos x}=\frac1{a+b}\sqrt{\frac{a+b}{b-a}}\ln|\frac{\tan\frac x2+\sqrt{\frac{a+b}{b-a}}}{\tan\frac x2-\sqrt{\frac{a+b}{b-a}}}|+C$ $(a^2$<  $b^2)$
<br/><br/>

107. $\int\frac{dx}{a^2\cos^2x+b^2\sin^2x}=\frac1{ab}\arctan(\frac ba\tan x)+C$
<br/><br/>

108. $\int\frac{dx}{a^2\cos^2x-b^2\sin^2x}=\frac1{2ab}\ln|\frac{b\tan x+a}{b\tan x-a}|+C$
<br/><br/>

109. $\int x\sin axdx=\frac1{a^2}\sin ax-\frac1ax\cos ax+C$
<br/><br/>

110. $\int x^2\sin axdx=-\frac1ax^2\cos ax+\frac2{a^2}x\sin ax+\frac2{a^3}\cos ax+C$
<br/><br/>

111. $\int x\cos axdx=\frac1{a^2}\cos ax+\frac 1ax\sin ax+C$
<br/><br/>

112. $\int x^2\cos axdx=\frac1ax^2\sin ax+\frac2{a^2}x\cos ax-\frac2{a^3}\sin ax+C$
<br/><br/>

## （十二）、含有反三角函数的积分(其中a>0)

113. $\int\arcsin\frac xadx=x\arcsin\frac xa+\sqrt{a^2-x^2}+C$
<br/><br/>

114. $\int x\arcsin\frac xadx=(\frac{x^2}{2}-\frac{a^2}4)\arcsin\frac xa+\frac x4\sqrt{a^2-x^2}+C$
<br/><br/>

115. $\int x^2\arcsin\frac xadx=\frac{x^3}3\arcsin\frac xa+\frac19(x^2+2a^2)\sqrt{a^2-x^2}+C$
<br/><br/>

116. $\int\arccos\frac xadx=x\arccos\frac xa-\sqrt{a^2-x^2}+C$
<br/><br/>

117. $\int x\arccos\frac xadx=(\frac{x^2}2-\frac{a^2}4)\arccos\frac xa-\frac x4\sqrt{a^2-x^2}+C$
<br/><br/>

118. $\int x^2\arccos\frac xadx=\frac{x^3}3\arccos\frac xa-\frac19(x^2+2a^2)\sqrt{a^2-x^2}+C$
<br/><br/>

119. $\int\arctan\frac xadx=x\arctan\frac xa-\frac a2\ln(a^2+x^2)+C$
<br/><br/>

120. $\int x\arctan\frac xadx=\frac12(a^2+x^2)\arctan\frac xa-\frac a2x+C$
<br/><br/>

121. $\int x^2\arctan\frac xadx=\frac{x^3}3\arctan\frac xa-\frac a6x^2+\frac{a^3}6\ln(a^2+x^2)+C$
<br/><br/>

## （十三）、含有指数函数的积分

122. $\int a^xdx=\frac1{\ln a}a^x+C$
<br/><br/>

123. $\int e^{ax}dx=\frac 1ae^{ax}+C$
<br/><br/>

124. $\int xe^{ax}dx=\frac1{a^2}(ax-1)e^{ax}+C$
<br/><br/>

125. $\int x^ne^{ax}dx=\frac1ax^ne^{ax}-\frac na\int x^{n-1}e^{ax}dx$
<br/><br/>

126. $\int xa^xdx=\frac x{\ln a}a^x-\frac1{(\ln a)^2}a^x+C$
<br/><br/>

127. $\int x^na^xdx=\frac1{\ln a}x^na^x-\frac n{\ln a}\int x^{n-1}a^xdx$
<br/><br/>

128. $\int e^{ax}\sin bxdx=\frac1{a^2+b^2}e^{ax}(a\sin bx-b\cos bx)+C$
<br/><br/>

129. $\int e^{ax}\cos bxdx=\frac1{a^2+b^2}e^{ax}(b\sin bx+a\cos bx)+C$
<br/><br/>

130. $\int e^{ax}\sin^nbxdx=\frac1{a^2+b^2n^2}e^{ax}\sin^{n-1}bx(a\sin bx-nb\cos bx)+\frac{n(n-1)b^2}{a^2+b^2n^2}\int e^{ax}\sin^{n-2}bxdx$
<br/><br/>

131. $\int e^{ax}\cos^nbxdx=\frac1{a^2+b^2n^2}e^{ax}\cos^{n-1}bx(a\cos bx+nb\sin bx)+\frac{n(n-1)b^2}{a^2+b^2n^2}\int e^{ax}\cos^{n-2}bxdx$
<br/><br/>

## （十四）、含有对数函数的积分

132. $\int\ln xdx=x\ln x-x+C$
<br/><br/>

133. $\int\frac{dx}{x\ln x}=\ln|\ln x|+C$
<br/><br/>

134. $\int x^n\ln xdx=\frac1{n+1}x^{n+1}(\ln x-\frac1{n+1})+C$
<br/><br/>

135. $\int(\ln x)^ndx=x(\ln x)^n-n\int(\ln x)^{n-1}dx$
<br/><br/>

136. $\int x^m(\ln x)^ndx=\frac1{m+1}x^{m+1}(\ln x)^n-\frac{n}{m+1}\int x^m(\ln x)^{n-1}dx$
<br/><br/>

## （十五）、含有双曲函数的积分

137. $\int sh xdx=ch x+C$
<br/><br/>

138. $\int ch xdx=sh x+C$
<br/><br/>

139. $\int th xdx=\ln ch x+C$
<br/><br/>

140. $\int sh^2xdx=-\frac x2+\frac14sh2x+C$
<br/><br/>

141. $\int ch^xdx=\frac x2+\frac14 sh2x+C$
<br/><br/>

## （十六）、定积分

142. $\int_{-\pi}^{\pi}\:\cos nxdx=\int_{-\pi}^{\pi}\sin nxdx=0$
<br/><br/>

143. $\int_{-\pi}^{\pi}\:\cos mx\sin nxdx=0$
<br/><br/>

144. $\int_{-\pi}^{\pi}\:\cos mx\cos nxdx=\begin{cases}0,m\neq n,\\\\ \pi,m=n.\end{cases}$
<br/><br/>

145. $\int_{-\pi}^{\pi}\:\sin mx\sin nxdx=\begin{cases}0,m\neq n,\\\\ \pi,m=n.\end{cases}$
<br/><br/>

146. $\int_{0}^{\pi}\sin mx\sin nxdx=\int_0^{\pi}\cos mx\cos nxdx$

$=\begin{cases}0,m\neq n,\\\\ \frac{\pi}2,m=n.\end{cases}$
<br/><br/>

147. $I_n=\int_0^{\frac{\pi}2}\:\sin^nxdx=\int_0^{\frac{\pi}2}\cos^nxdx,$
<br/>

$I_n=\frac{n-1}nI_{n-2}$
<br/>

$=\begin{cases}\frac{n-1}n\cdot\frac{n-3}{n-2}\cdot\,\cdots\,\cdot\frac45\cdot\frac23(n为大于1的正奇数),I_1=1,\\\\ \frac{n-1}n\cdot\frac{n-3}{n-2}\cdot\,\cdots\,\cdot\frac34\cdot\frac12\cdot\frac{\pi}2(n为正偶数),I_0=\frac{\pi}2. \end{cases}$





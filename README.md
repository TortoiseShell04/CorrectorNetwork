# Corrector Network
## How it works 
It uses multi head similarity to predict similarity using different methods, then concats the vectors into a matrix of size NxH <br>
<math xmlns="http://www.w3.org/1998/Math/MathML"><mi>M</mi><mo>&#x2022;</mo><mi>U</mi><mo>&#xA0;</mo><mo>=</mo><mo>&#xA0;</mo><mi>O</mi><mi>u</mi><mi>t</mi><mi>U</mi><mi>X</mi></math><br>
<math xmlns="http://www.w3.org/1998/Math/MathML"><mi>O</mi><mi>u</mi><mi>t</mi><mi>U</mi><mi>X</mi><mo>&#x2022;</mo><mi>V</mi><mo>&#xA0;</mo><mo>=</mo><mo>&#xA0;</mo><mi>O</mi><mi>u</mi><mi>t</mi><mi>U</mi><mi>V</mi></math><br>
<math xmlns="http://www.w3.org/1998/Math/MathML"><mi>O</mi><mi>u</mi><mi>t</mi><mi>p</mi><mi>u</mi><mi>t</mi><mo>&#xA0;</mo><mo>=</mo><mo>&#xA0;</mo><mi>s</mi><mi>o</mi><mi>f</mi><mi>t</mi><mi>m</mi><mi>a</mi><mi>x</mi><mo>(</mo><mi>O</mi><mi>u</mi><mi>t</mi><mi>p</mi><mi>u</mi><mi>t</mi><mi>X</mi><mi>V</mi><mo>)</mo></math><br>
## Back propagation
<math xmlns="http://www.w3.org/1998/Math/MathML"><mfrac><mrow><mo>&#x2202;</mo><mi>L</mi></mrow><mrow><mo>&#x2202;</mo><mi>/V</mi></mrow></mfrac><mo>&#xA0;</mo><mo>=</mo><mo>&#xA0;</mo><mfrac><mrow><mo>&#x2202;</mo><mi>L</mi></mrow><mrow><mo>&#x2202;</mo><mi>/O</mi></mrow></mfrac><mo>&#x2022;</mo><mfrac><mrow><mo>&#x2202;</mo><mi>O</mi></mrow><mrow><mo>&#x2202;</mo><mi>/O</mi><mi>u</mi><mi>t</mi><mi>p</mi><mi>u</mi><mi>t</mi><mi>X</mi><mi>V</mi></mrow></mfrac><mo>&#x2022;</mo><mfrac><mrow><mo>&#x2202;</mo><mi>O</mi><mi>u</mi><mi>t</mi><mi>p</mi><mi>u</mi><mi>t</mi><mi>X</mi><mi>V</mi></mrow><mrow><mo>&#x2202;</mo><mi>/V</mi></mrow></mfrac></math><br>
<math xmlns="http://www.w3.org/1998/Math/MathML"><mfrac><mrow><mo>&#x2202;</mo><mi>L</mi></mrow><mrow><mo>&#x2202;</mo><mi>U</mi></mrow></mfrac><mo>&#xA0;</mo><mo>=</mo><mo>&#xA0;</mo><mfrac><mrow><mo>&#x2202;</mo><mi>L</mi></mrow><mrow><mo>&#x2202;</mo><mi>O</mi></mrow></mfrac><mo>&#x2022;</mo><mfrac><mrow><mo>&#x2202;</mo><mi>O</mi></mrow><mrow><mo>&#x2202;</mo><mi>O</mi><mi>u</mi><mi>t</mi><mi>p</mi><mi>u</mi><mi>t</mi><mi>X</mi><mi>V</mi></mrow></mfrac><mo>&#x2022;</mo><mfrac><mrow><mo>&#x2202;</mo><mi>O</mi><mi>u</mi><mi>t</mi><mi>p</mi><mi>u</mi><mi>t</mi><mi>X</mi><mi>V</mi></mrow><mrow><mo>&#x2202;</mo><mi>O</mi><mi>u</mi><mi>t</mi><mi>p</mi><mi>u</mi><mi>t</mi><mi>X</mi><mi>U</mi></mrow></mfrac><mo>&#x2022;</mo><mfrac><mrow><mo>&#x2202;</mo><mi>O</mi><mi>u</mi><mi>t</mi><mi>p</mi><mi>u</mi><mi>t</mi><mi>X</mi><mi>U</mi></mrow><mrow><mo>&#x2202;</mo><mi>U</mi></mrow></mfrac></math>

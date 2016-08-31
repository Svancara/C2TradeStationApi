<h1>Trading signals from TradeStation to Collective2.</h1>

<p>Purpose of this work is to make communication between TradeStation and Collective2 more reliable. 
Currently used SMTP communication is error prone and we need a better solution.</p>

<p>
  A new idea: Use Collective2 Signals API.
</p>
      
<p>Collective2 Api is described here: <a href="https://collective2.com/api-docs/latest" target="_blank" title="Collective2 API">https://collective2.com/api-docs/latest</a></p>      

<p>Initial commit includes these files:</p>

<ul>
  <li><p>
        c2api_globals.txt
      </p>
      <p>
        Global constants. Do not touch them. Those must be the same on both sides.
      </p>
      </li>
  <li><p>
        c2api_key.txt
      </p>
      <p>
        A one-line function holding user's Collective Api key. Enter your Collectiv2 API key here.
      </p>
      </li>
  <li><p>
        c2api_SendSignal.txt
      </p>
      <p>
        Implementation of Collective2 Api submitSignal function (<a href="https://collective2.com/api-signal-entry#toc-submitsignal">https://collective2.com/api-signal-entry#toc-submitsignal</a>)
        in EasyLanguage.
      </p>
      </li>
  <li>
  <p>
    c2api_v3_indicator.txt
  </p>
  <p>
    Backbone of TradeStation indicator. 
  </p>
  </li>
  
</ul>

<p>But it will not work. TradeStation does not allow inputs nad local varibles as arguments to separate functions. Huh!</p>

<p>A new 'all in one' solution is in the file <i>c2api_v3_indicator_new_01.txt</i> .</p>

<p>It partially works. But we need to test it if it is usable. Then - we need to add remaining functionality. </p>


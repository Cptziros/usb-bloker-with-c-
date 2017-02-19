<h1>USB Port Blocker With C#</h1>

<h2>Introduction</h2>

<p>USB Port Blocker is a simple thing in the computer programming, and this program can disable &amp; enable your computer USB ports from Registry - Have fun! *_^</p>

<p>&nbsp;</p>

<h2>How it works?</h2>

<p>it&#39;s working with 2 Using Keywords&nbsp;For disable &amp; enable USB you need to change registry values programmatically.</p>

<p>following the codes :</p>

<div class="pre-action-link" id="premain269918" style="width:100%;display:block;"><span id="prehide269918" onclick="processCodeBlocks.togglePre(269918);">Hide</span> &nbsp; <span id="copycode269918" onclick="return processCodeBlocks.copyCode(269918);">Copy Code</span></div>

<pre class="notranslate" id="pre269918" lang="C#" style="margin-top: 0px;">
<strong><span class="code-keyword"> using</span> System.Security.Permissions;</strong>
<strong><span class="code-keyword"> using</span> Microsoft.Win32; </strong>
 </pre>

<div class="text"><br />
<br />
<br />
For disable USB :</div>

<div class="pre-action-link" id="premain269918" style="width:100%;display:block;"><span id="prehide269918" onclick="processCodeBlocks.togglePre(269918);">Hide</span> &nbsp; <span id="copycode269918" onclick="return processCodeBlocks.copyCode(269918);">Copy Code</span></div>

<pre class="notranslate" id="pre269918" lang="C#" style="margin-top: 0px;">
Microsoft.Win32.Registry.SetValue(<span class="code-string">@&quot;</span><span class="code-string">HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\USBSTOR&quot;</span>, <span class="code-string">&quot;</span><span class="code-string">Start&quot;</span>, <span class="code-digit">4</span>, Microsoft.Win32.RegistryValueKind.DWord);
 </pre>

<p><br />
For enable USB :</p>

<p>&nbsp;</p>

<div class="pre-action-link" id="premain880138" style="width:100%;display:block;"><span id="prehide880138" onclick="processCodeBlocks.togglePre(880138);">Hide</span> &nbsp; <span id="copycode880138" onclick="return processCodeBlocks.copyCode(880138);">Copy Code</span></div>

<p>&nbsp;</p>

<pre class="notranslate" id="pre880138" lang="C#" style="margin-top: 0px;">
Microsoft.Win32.Registry.SetValue(<span class="code-string">@&quot;</span><span class="code-string">HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\USBSTOR&quot;</span>, <span class="code-string">&quot;</span><span class="code-string">Start&quot;</span>, <span class="code-digit">3</span>, Microsoft.Win32.RegistryValueKind.DWord);</pre>

<div>&nbsp;</div>

<div>Ok , for last words it program must be running as Administrator.</div>

<p>&nbsp;</p>


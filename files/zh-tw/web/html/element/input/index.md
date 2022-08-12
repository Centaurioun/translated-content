---
title: <input>
slug: Web/HTML/Element/input
tags:
  - Element
  - Forms
  - HTML
  - HTML forms
  - HTML input tag
  - MakeBrowserAgnostic
  - NeedsBrowserCompatibility
  - NeedsMobileBrowserCompatibility
  - NeedsTranslation
  - Reference
  - TopicStub
  - Web
translation_of: Web/HTML/Element/input
---
<div>{{HTMLRef}}</div>

<p>The <strong>HTML <code>&lt;input&gt;</code> element</strong> is used to create interactive controls for web-based forms in order to accept data from the user.</p>

<h2 id="Live_example">Live example</h2>

<p>To get an idea of how different the various <code>&lt;input&gt;</code> types look, try editing the value of the <code>type</code> attributes in the following editable live example; you'll see the output update as you type. In each case, the initial value (<code>text</code>) produces a basic text input, but you can try other values such as <code>number</code>, <code>color</code>, <code>checkbox</code>, <code>radio</code>, <code>date</code>, <code>file</code>, <code>month</code>, <code>password</code>, <code>range</code>, or <code>time</code>.</p>

<p>{{EmbedGHLiveSample("learning-area/html/forms/editable-input-example/editable_input.html", '100%', 230)}}</p>

<table class="properties">
 <tbody>
  <tr>
   <th scope="row"><a href="/en-US/docs/HTML/Content_categories">Content categories</a></th>
   <td><a href="/en-US/docs/HTML/Content_categories#Flow_content">Flow content</a>, listed, submittable, resettable, form-associated element, <a href="/en-US/docs/HTML/Content_categories#Phrasing_content">phrasing content</a>. If the {{htmlattrxref("type", "input")}} is not <code>hidden</code>, then labellable element, palpable content.</td>
  </tr>
  <tr>
   <th scope="row">Permitted content</th>
   <td>None, it is an {{Glossary("empty element")}}.</td>
  </tr>
  <tr>
   <th scope="row">Tag omission</th>
   <td>Must have a start tag and must not have an end tag.</td>
  </tr>
  <tr>
   <th scope="row">Permitted parents</th>
   <td>Any element that accepts <a href="/en-US/docs/HTML/Content_categories#Phrasing_content">phrasing content</a>.</td>
  </tr>
  <tr>
   <th scope="row">Permitted ARIA roles</th>
   <td>
    <ul>
     <li><code>type=button</code>: {{ARIARole("link")}}, {{ARIARole("menuitem")}}, {{ARIARole("menuitemcheckbox")}}, {{ARIARole("menuitemradio")}}, {{ARIARole("radio")}}, {{ARIARole("switch")}}, {{ARIARole("tab")}}</li>
     <li><code>type=checkbox</code>: {{ARIARole("button")}}, {{ARIARole("menuitemcheckbox")}}, {{ARIARole("option")}}, {{ARIARole("switch")}}</li>
     <li><code>type=image</code>: {{ARIARole("link")}}, {{ARIARole("menuitem")}}, {{ARIARole("menuitemcheckbox")}}, {{ARIARole("menuitemradio")}}, {{ARIARole("radio")}}, {{ARIARole("switch")}}</li>
     <li><code>type=radio</code>: {{ARIARole("menuitemradio")}}</li>
     <li><code>type=color|date|datetime|datetime-local|email|file</code>: None</li>
     <li><code>type=hidden|month|number|password|range|research</code>: None</li>
     <li><code>type=search|submit|tel|text|url|week</code>: None</li>
    </ul>
   </td>
  </tr>
  <tr>
   <th scope="row">DOM interface</th>
   <td>{{domxref("HTMLInputElement")}}</td>
  </tr>
 </tbody>
</table>

<h2 id="Form_&lt;input>_types">Form <code>&lt;input&gt;</code> types</h2>

<p>How an <code>&lt;input&gt;</code> works varies considerably depending on the value of its <code>type</code> attribute, hence the different types are covered in their own separate reference pages. If this attributes is not specified, the default type adopted type is <code>text</code>.</p>

<p>The available types are as follows:</p>

<ul>
 <li><code><a href="/en-US/docs/Web/HTML/Element/input/button">button</a></code>: A push button with no default behavior.</li>
 <li><code><a href="/en-US/docs/Web/HTML/Element/input/checkbox">checkbox</a></code>: A check box allowing single values to be selected/deselected.</li>
 <li><code><a href="/en-US/docs/Web/HTML/Element/input/color">color</a></code>: A control for specifying a color. A color picker's UI has no required features other than accepting simple colors as text (<a href="https://www.w3.org/TR/html5/forms.html#color-state-(type=color)">more info</a>).</li>
 <li><code><a href="/en-US/docs/Web/HTML/Element/input/date">date</a></code>: A control for entering a date (year, month, and day, with no time).</li>
 <li><code><a href="/en-US/docs/Web/HTML/Element/input/datetime-local">datetime-local</a></code>: A control for entering a date and time, with no time zone.</li>
 <li><code><a href="/en-US/docs/Web/HTML/Element/input/email">email</a></code>: A field for editing an e-mail address.</li>
 <li><code><a href="/en-US/docs/Web/HTML/Element/input/file">file</a></code>: A control that lets the user select a file. Use the <strong>accept</strong> attribute to define the types of files that the control can select.</li>
 <li><code><a href="/en-US/docs/Web/HTML/Element/input/hidden">hidden</a></code>: A control that is not displayed but whose value is submitted to the server.</li>
 <li><code><a href="/en-US/docs/Web/HTML/Element/input/image">image</a></code>: A graphical submit button. You must use the <strong>src</strong> attribute to define the source of the image and the <strong>alt</strong> attribute to define alternative text. You can use the <strong>height</strong> and <strong>width</strong> attributes to define the size of the image in pixels.</li>
 <li><code><a href="/en-US/docs/Web/HTML/Element/input/month">month</a></code>: A control for entering a month and year, with no time zone.</li>
 <li><code><a href="/en-US/docs/Web/HTML/Element/input/number">number</a></code>: A control for entering a number.</li>
 <li><code><a href="/en-US/docs/Web/HTML/Element/input/password">password</a></code>: A single-line text field whose value is obscured. Use the <strong>maxlength</strong> attribute to specify the maximum length of the value that can be entered.
  <div class="note"><strong>Note</strong>: Any forms involving sensitive information like passwords (e.g. login forms) should be served over HTTPS; Firefox now implements multiple mechanisms to warn against insecure login forms — see <a href="/en-US/docs/Web/Security/Insecure_passwords">Insecure passwords</a>. Other browsers are also implementing similar mechanisms.</div>
 </li>
 <li><code><a href="/en-US/docs/Web/HTML/Element/input/radio">radio</a></code>: A radio button, allowing a single value to be selected out of multiple choices.</li>
 <li><code><a href="/en-US/docs/Web/HTML/Element/input/range">range</a></code>: A control for entering a number whose exact value is not important.</li>
 <li><code><a href="/en-US/docs/Web/HTML/Element/input/reset">reset</a></code>: A button that resets the contents of the form to default values.</li>
 <li><code><a href="/en-US/docs/Web/HTML/Element/input/search">search</a></code>: A single-line text field for entering search strings. Line-breaks are automatically removed from the input value.</li>
 <li><code><a href="/en-US/docs/Web/HTML/Element/input/submit">submit</a></code>: A button that submits the form.</li>
 <li><code><a href="/en-US/docs/Web/HTML/Element/input/tel">tel</a></code>: A control for entering a telephone number. Line-breaks are automatically removed from the input value, but no other syntax is enforced. You can use attributes such as <strong>pattern</strong> and <strong>maxlength</strong> to restrict values entered in the control. The {{cssxref(":valid")}} and {{cssxref(":invalid")}} CSS pseudo-classes are applied as appropriate.</li>
 <li><code><a href="/en-US/docs/Web/HTML/Element/input/text">text</a></code>: A single-line text field. Line-breaks are automatically removed from the input value.</li>
 <li><code><a href="/en-US/docs/Web/HTML/Element/input/time">time</a></code>: A control for entering a time value with no time zone.</li>
 <li><code><a href="/en-US/docs/Web/HTML/Element/input/url">url</a></code>: A field for editing a URL. The input value is validated to contain either the empty string or a valid absolute URL before submitting. You can use attributes such as <strong>pattern</strong> and <strong>maxlength</strong> to restrict values entered in the control. The {{cssxref(":valid")}} and {{cssxref(":invalid")}} CSS pseudo-classes are applied as appropriate.</li>
 <li><code><a href="/en-US/docs/Web/HTML/Element/input/week">week</a></code>: A control for entering a date consisting of a week-year number and a week number with no time zone.</li>
</ul>

<p>Some input types are now obsolete:</p>

<ul>
 <li><code><a href="/en-US/docs/Web/HTML/Element/input/datetime">datetime</a></code>: {{deprecated_inline}} A control for entering a date and time (hour, minute, second, and fraction of a second) based on UTC time zone. <strong>This feature has been <a href="https://github.com/whatwg/html/issues/336">removed from WHATWG HTML.</a></strong></li>
</ul>

<h2 id="Attributes">Attributes</h2>

<h3 id="Global_&lt;input>_attributes">Global <code>&lt;input&gt;</code> attributes</h3>

<p>This section lists the attributes available to all form <code>&lt;input&gt;</code> types. Non-global attributes — and global attributes that behave differently when specified on different <code>&lt;input&gt;</code> types — are listed on those types' individual pages.</p>

<div class="note">
<p><strong>Note</strong>: This includes the <a href="/en-US/docs/Web/HTML/Global_attributes">global HTML attributes</a>.</p>
</div>

<dl>
 <dt>{{htmlattrdef("type")}}</dt>
 <dd>The type of control to render. See <a href="#form_&lt;input>_types">Form &lt;input&gt; types</a> for the individual types, with links to more information about each.</dd>
 <dt>{{htmlattrdef("accept")}}</dt>
 <dd>If the value of the <strong>type</strong> attribute is <code>file</code>, then this attribute will indicate the types of files that the server accepts, otherwise it will be ignored. The value must be a comma-separated list of unique content type specifiers:
 <ul>
  <li>A file extension starting with the STOP character (U+002E). (e.g. .jpg, .png, .doc).</li>
  <li>A valid MIME type with no extensions.</li>
  <li><code>audio/*</code> representing sound files.</li>
  <li><code>video/*</code> representing video files.</li>
  <li><code>image/*</code> representing image files.</li>
 </ul>
 </dd>
 <dt>{{htmlattrdef("accesskey")}} {{Deprecated_Inline}}</dt>
 <dd>A single-character that the user can press to switch input focus to the control. This attribute is global in HTML5.</dd>
 <dt>{{htmlattrdef("autocomplete")}}</dt>
 <dd>This attribute indicates whether the value of the control can be automatically completed by the browser. Possible values are:
 <ul>
  <li><code>off</code>: The user must explicitly enter a value into this field for every use, or the document provides its own auto-completion method. The browser does not automatically complete the entry.</li>
  <li><code>on</code>: The browser is allowed to automatically complete the value based on values that the user has entered during previous uses, however <code>on</code> does not provide any further information about what kind of data the user might be expected to enter.</li>
  <li><code>name</code>: Full name.</li>
  <li><code>honorific-prefix: </code>Prefix or title (e.g. "Mr.", "Ms.", "Dr.", "Mlle").</li>
  <li><code>given-name</code>: First name.</li>
  <li><code>additional-name</code>: Middle name.</li>
  <li><code>family-name</code>: Last name.</li>
  <li><code>honorific-suffix</code>: Suffix (e.g. "Jr.", "B.Sc.", "MBASW", "II").</li>
  <li><code>nickname</code></li>
  <li><code>email</code></li>
  <li><code>username</code></li>
  <li><code>new-password</code>: A new password (e.g. when creating an account or changing a password).</li>
  <li><code>current-password</code></li>
  <li><code>organization-title</code>: Job title (e.g. "Software Engineer", "Senior Vice President", "Deputy Managing Director").</li>
  <li><code>organization</code></li>
  <li><code>street-address</code></li>
  <li><code>address-line1</code>, <code>address-line2</code>, <code>address-line3</code>, <code>address-level4</code>, <code>address-level3</code>, <code>address-level2</code>, <code>address-level1</code></li>
  <li><code>country</code></li>
  <li><code>country-name</code></li>
  <li><code>postal-code</code></li>
  <li><code>cc-name</code>: Full name as given on the payment instrument.</li>
  <li><code>cc-given-name</code></li>
  <li><code>cc-additional-name</code></li>
  <li><code>cc-family-name</code></li>
  <li><code>cc-number</code>: Code identifying the payment instrument (e.g. the credit card number).</li>
  <li><code>cc-exp:</code> Expiration date of the payment instrument.</li>
  <li><code>cc-exp-month</code></li>
  <li><code>cc-exp-year</code></li>
  <li><code>cc-csc</code>: Security code for the payment instrument.</li>
  <li><code>cc-type</code>: Type of payment instrument (e.g. Visa).</li>
  <li><code>transaction-currency</code></li>
  <li><code>transaction-amount</code></li>
  <li><code>language</code>: Preferred language; a valid <a href="https://en.wikipedia.org/wiki/IETF_language_tag">BCP 47 language tag</a>.</li>
  <li><code>bday</code>: birthday</li>
  <li><code>bday-day</code></li>
  <li><code>bday-month</code></li>
  <li><code>bday-year</code></li>
  <li><code>sex</code>: Gender identity (e.g. Female, Fa'afafine), free-form text, no newlines.</li>
  <li><code>tel</code>: full telephone number, including country code
   <ul>
    <li>additional <code>tel</code> variants: <code>tel-country-code</code>, <code>tel-national</code>, <code>tel-area-code</code>, <code>tel-local</code>, <code>tel-local-prefix</code>, <code>tel-local-suffix</code>, <code>tel-extension</code></li>
   </ul>
  </li>
  <li><code>url</code>: Home page or other Web page corresponding to the company, person, address, or contact information in the other fields associated with this field.</li>
  <li><code>photo</code>: Photograph, icon, or other image corresponding to the company, person, address, or contact information in the other fields associated with this field.</li>
 </ul>

 <p>See the <a href="https://html.spec.whatwg.org/multipage/forms.html#autofill">WHATWG Standard</a> for more detailed information.</p>

 <p>If the <strong>autocomplete</strong> attribute is not specified on an input element then the browser uses the <strong>autocomplete</strong> attribute value of the <code>&lt;input&gt;</code> element's form owner. The form owner is either the <code>form</code> element that this <code>&lt;input&gt;</code> element is a descendant of or the form element whose <strong>id</strong> is specified by the <strong>form</strong> attribute of the input element. For more information, see the {{htmlattrxref("autocomplete", "form")}} attribute in {{HTMLElement("form")}}.</p>

 <p>The <strong>autocomplete</strong> attribute also controls whether Firefox will, unlike other browsers, <a href="https://stackoverflow.com/questions/5985839/bug-with-firefox-disabled-attribute-of-input-not-resetting-when-refreshing">persist the dynamic disabled state and (if applicable) dynamic checkedness</a> of an <code>&lt;input&gt;</code> across page loads. The persistence feature is enabled by default. Setting the value of the <strong>autocomplete</strong> attribute to <code>off</code> disables this feature. This works even when the <strong>autocomplete</strong> attribute would normally not apply to the <code>&lt;input&gt;</code> by virtue of its <strong>type</strong>. See {{bug(654072)}}.</p>

 <p>For most modern browsers (including Firefox 38+, Google Chrome 34+, IE 11+), setting the <strong>autocomplete</strong> attribute will <em>not</em> prevent a browser's password manager from asking the user if they want to store login (username and password) fields and, if they agree, from autofilling the login the next time the user visits the page. See <a href="/en-US/docs/Web/Security/Securing_your_site/Turning_off_form_autocompletion#The_autocomplete_attribute_and_login_fields">the autocomplete attribute and login fields</a>.</p>
 </dd>
 <dt>{{htmlattrdef("autofocus")}}</dt>
 <dd>This Boolean attribute lets you specify that a form control should have input focus when the page loads, unless the user overrides it (e.g. by typing in a different control). Only one form element in a document can have the <strong>autofocus</strong> attribute, which is a Boolean. It cannot be applied if the <strong>type</strong> attribute is set to <code>hidden</code> (that is, you cannot automatically set focus to a hidden control). Note that the focusing of the control may occur before the firing of the <a href="/en-US/docs/Web/Events/DOMContentLoaded"><code>DOMContentLoaded</code> event.</a></dd>
 <dt>{{htmlattrdef("capture")}}</dt>
 <dd>
 <p>When the value of the <strong>type</strong> attribute is <code>file</code>, the presence of this Boolean attribute indicates that capture of media directly from the device's environment using a <a href="https://www.w3.org/TR/html-media-capture/#dfn-media-capture-mechanism">media capture mechanism</a> is preferred.</p>
 </dd>
 <dt>{{htmlattrdef("checked")}}</dt>
 <dd>
 <p>When the value of the <strong>type</strong> attribute is <code>radio</code> or <code>checkbox</code>, the presence of this Boolean attribute indicates that the control is selected by default, otherwise it is ignored.</p>

 <p>Unlike other browsers, Firefox will by default <a href="https://stackoverflow.com/questions/5985839/bug-with-firefox-disabled-attribute-of-input-not-resetting-when-refreshing">persist the dynamic checked state</a> of an <code>&lt;input&gt;</code> across page loads. Use the {{htmlattrxref("autocomplete","input")}} attribute to control this feature.</p>
 </dd>
 <dt>{{htmlattrdef("disabled")}}</dt>
 <dd>
 <p>This Boolean attribute indicates that the form control is not available for interaction. In particular, the <code>click</code> event <a href="https://html.spec.whatwg.org/multipage/forms.html#enabling-and-disabling-form-controls:-the-disabled-attribute">will not be dispatched</a> on disabled controls. Also, a disabled control's value isn't submitted with the form.</p>

 <p>Unlike other browsers, Firefox will by default <a href="https://stackoverflow.com/questions/5985839/bug-with-firefox-disabled-attribute-of-input-not-resetting-when-refreshing">persist the dynamic disabled state</a> of an <code>&lt;input&gt;</code> across page loads. Use the {{htmlattrxref("autocomplete","input")}} attribute to control this feature.</p>
 </dd>
 <dt>{{htmlattrdef("form")}}</dt>
 <dd>The form element that the input element is associated with (its <em>form owner</em>). The value of the attribute must be an <strong>id</strong> of a {{HTMLElement("form")}} element in the same document. If this attribute is not specified, this <code>&lt;input&gt;</code> element must be a descendant of a {{HTMLElement("form")}} element. This attribute enables you to place <code>&lt;input&gt;</code> elements anywhere within a document, not just as descendants of their form elements. An input can only be associated with one form.</dd>
 <dt>{{htmlattrdef("formaction")}}</dt>
 <dd>The URI of a program that processes the information submitted by the input element, if it is a submit button or image. If specified, it overrides the {{htmlattrxref("action","form")}} attribute of the element's form owner.</dd>
 <dt>{{htmlattrdef("formenctype")}}</dt>
 <dd>If the input element is a submit button or image, this attribute specifies the type of content that is used to submit the form to the server. Possible values are:
 <ul>
  <li><code>application/x-www-form-urlencoded</code>: The default value if the attribute is not specified.</li>
  <li><code>multipart/form-data</code>: Use this value if you are using an <code>&lt;input&gt;</code> element with the {{htmlattrxref("type","input")}} attribute set to <code>file</code>.</li>
  <li><code>text/plain</code></li>
 </ul>

 <p>If this attribute is specified, it overrides the {{htmlattrxref("enctype","form")}} attribute of the element's form owner.</p>
 </dd>
 <dt>{{htmlattrdef("formmethod")}}</dt>
 <dd>If the input element is a submit button or image, this attribute specifies the HTTP method that the browser uses to submit the form. Possible values are:
 <ul>
  <li><code>post</code>: The data from the form is included in the body of the form and is sent to the server.</li>
  <li><code>get</code>: The data from the form are appended to the <strong>form</strong> attribute URI, with a '?' as a separator, and the resulting URI is sent to the server. Use this method when the form has no side-effects and contains only ASCII characters.</li>
 </ul>

 <p>If specified, this attribute overrides the {{htmlattrxref("method","form")}} attribute of the element's form owner.</p>
 </dd>
 <dt>{{htmlattrdef("formnovalidate")}}</dt>
 <dd>If the input element is a submit button or image, this Boolean attribute specifies that the form is not to be validated when it is submitted. If this attribute is specified, it overrides the {{htmlattrxref("novalidate","form")}} attribute of the element's form owner.</dd>
 <dt>{{htmlattrdef("formtarget")}}</dt>
 <dd>If the input element is a submit button or image, this attribute is a name or keyword indicating where to display the response that is received after submitting the form. This is a name of, or keyword for, a <em>browsing context</em> (e.g. tab, window, or inline frame). If this attribute is specified, it overrides the {{htmlattrxref("target", "form")}} attribute of the elements's form owner. The following keywords have special meanings:
 <ul>
  <li>_<code>self</code>: Load the response into the same browsing context as the current one. This value is the default if the attribute is not specified.</li>
  <li><code>_blank</code>: Load the response into a new unnamed browsing context.</li>
  <li><code>_parent</code>: Load the response into the parent browsing context of the current one. If there is no parent, this option behaves the same way as <code>_self</code>.</li>
  <li><code>_top</code>: Load the response into the top-level browsing context (i.e. the browsing context that is an ancestor of the current one, and has no parent). If there is no parent, this option behaves the same way as <code>_self</code>.</li>
 </ul>
 </dd>
 <dt>{{htmlattrdef("height")}}</dt>
 <dd>If the value of the <strong>type</strong> attribute is <code>image</code>, this attribute defines the height of the image displayed for the button.</dd>
 <dt>{{htmlattrdef("inputmode")}}</dt>
 <dd>A hint to the browser for which keyboard to display. This attribute applies when the value of the <strong>type</strong> attribute is text, password, email, or url. Possible values are:
 <ul>
  <li><code>verbatim</code>: Alphanumeric, non-prose content such as usernames and passwords.</li>
  <li><code>latin</code>: Latin-script input in the user's preferred language with typing aids such as text prediction enabled. For human-to-computer communication such as search boxes.</li>
  <li><code>latin-name</code>: As <em>latin</em>, but for human names.</li>
  <li><code>latin-prose</code>: As <em>latin</em>, but with more aggressive typing aids. For human-to-human communication such as instant messaging or email.</li>
  <li><code>full-width-latin</code>: As <em>latin-prose</em>, but for the user's secondary languages.</li>
  <li><code>kana</code>: Kana or romaji input, typically hiragana input, using full-width characters, with support for converting to kanji. Intended for Japanese text input.</li>
  <li><code>katakana</code>: Katakana input, using full-width characters, with support for converting to kanji. Intended for Japanese text input.</li>
  <li><code>numeric</code>: Numeric input, including keys for the digits 0 to 9, the user's preferred thousands separator character, and the character for indicating negative numbers. Intended for numeric codes (e.g. credit card numbers). For actual numbers, prefer using &lt;input type="number"&gt;</li>
  <li><code>tel</code>: Telephone input, including asterisk and pound key. Use &lt;input type="tel"&gt; if possible instead.</li>
  <li><code>email</code>: Email input. Use &lt;input type="email"&gt; if possible instead.</li>
  <li><code>url</code>: URL input. Use &lt;input type="url"&gt; if possible instead.</li>
 </ul>
 </dd>
 <dt>{{htmlattrdef("list")}}</dt>
 <dd>Identifies a list of pre-defined options to suggest to the user. The value must be the <strong>id</strong> of a {{HTMLElement("datalist")}} element in the same document. The browser displays only options that are valid values for this input element. This attribute is ignored when the <strong>type</strong> attribute's value is <code>hidden</code>, <code>checkbox</code>, <code>radio</code>, <code>file</code>, or a button type.</dd>
 <dt>{{htmlattrdef("max")}}</dt>
 <dd>The maximum (numeric or date-time) value for this item, which must not be less than its minimum (<strong>min</strong> attribute) value.</dd>
 <dt>{{htmlattrdef("maxlength")}}</dt>
 <dd>If the value of the <strong>type</strong> attribute is <code>text</code>, <code>email</code>,<code> search</code>, <code>password</code>, <code>tel</code>, or <code>url</code>, this attribute specifies the maximum number of characters (in UTF-16 code units) that the user can enter. For other control types, it is ignored. It can exceed the value of the <strong>size</strong> attribute. If it is not specified, the user can enter an unlimited number of characters. Specifying a negative number results in the default behavior (i.e. the user can enter an unlimited number of characters). The constraint is evaluated only when the value of the attribute has been changed.</dd>
 <dt>{{htmlattrdef("min")}}</dt>
 <dd>The minimum (numeric or date-time) value for this item, which must not be greater than its maximum (<strong>max</strong> attribute) value.</dd>
 <dt>{{htmlattrdef("minlength")}}</dt>
 <dd>If the value of the <strong>type</strong> attribute is <code>text</code>, <code>email</code>,<code> search</code>, <code>password</code>, <code>tel</code>, or <code>url</code>, this attribute specifies the minimum number of characters (in Unicode code points) that the user can enter. For other control types, it is ignored.</dd>
 <dt>{{htmlattrdef("multiple")}}</dt>
 <dd>This Boolean attribute indicates whether the user can enter more than one value. This attribute applies when the <strong>type</strong> attribute is set to <code>email</code> or <code>file</code>, otherwise it is ignored.</dd>
 <dt>{{htmlattrdef("name")}}</dt>
 <dd>The name of the control, which is submitted with the form data.</dd>
 <dt>{{htmlattrdef("pattern")}}</dt>
 <dd>A regular expression that the control's value is checked against. The pattern must match the entire value, not just some subset. Use the <strong>title</strong> attribute to describe the pattern to help the user. This attribute applies when the value of the <strong>type</strong> attribute is <code>text</code>, <code>search</code>, <code>tel</code>, <code>url</code>, <code>email</code>, or <code>password</code>, otherwise it is ignored. The regular expression language is the same as JavaScript {{jsxref("RegExp")}} algorithm, with the <code>'u'</code> parameter that makes it treat the pattern as a sequence of unicode code points. The pattern is not surrounded by forward slashes.</dd>
 <dt>{{htmlattrdef("placeholder")}}</dt>
 <dd>A hint to the user of what can be entered in the control . The placeholder text must not contain carriage returns or line-feeds.
 <div class="note"><strong>Note:</strong> Do not use the <code>placeholder</code> attribute instead of a {{HTMLElement("label")}} element, their purposes are different. The {{HTMLElement("label")}} attribute describes the role of the form element (i.e. it indicates what kind of information is expected), and the <code>placeholder</code> attribute is a hint about the format that the content should take. There are cases in which the <code>placeholder</code> attribute is never displayed to the user, so the form must be understandable without it.</div>
 </dd>
 <dt>{{htmlattrdef("readonly")}}</dt>
 <dd>This attribute indicates that the user cannot modify the value of the control. The value of the attribute is irrelevant. If you need read-write access to the input value, <em>do not</em> add the "<strong>readonly</strong>" attribute. It is ignored if the value of the <strong>type</strong> attribute is <code>hidden</code>, <code>range</code>, <code>color</code>, <code>checkbox</code>, <code>radio</code>, <code>file</code>, or a button type (such as <code>button</code> or <code>submit</code>).</dd>
 <dt>{{htmlattrdef("required")}}</dt>
 <dd>This attribute specifies that the user must fill in a value before submitting a form. It cannot be used when the <strong>type</strong> attribute is <code>hidden</code>, <code>image</code>, or a button type (<code>submit</code>, <code>reset</code>, or <code>button</code>). The {{cssxref(":optional")}} and {{cssxref(":required")}} CSS pseudo-classes will be applied to the field as appropriate.</dd>
 <dt>{{htmlattrdef("selectionDirection")}}</dt>
 <dd>The direction in which selection occurred. This is <code>"forward"</code> if the selection was made from left-to-right in an LTR locale or right-to-left in an RTL locale, or <code>"backward"</code> if the selection was made in the opposite direction. On platforms on which it's possible this value isn't known, the value can be <code>"none"</code>; for example, on macOS, the default direction is <code>"none"</code>, then as the user begins to modify the selection using the keyboard, this will change to reflect the direction in which the selection is expanding.</dd>
 <dt>{{htmlattrdef("selectionEnd")}}</dt>
 <dd>The offset into the element's text content of the last selected character. If there's no selection, this value indicates the offset to the character following the current text input cursor position (that is, the position the next character typed would occupy).</dd>
 <dt>{{htmlattrdef("selectionStart")}}</dt>
 <dd>The offset into the element's text content of the first selected character. If there's no selection, this value indicates the offset to the character following the current text input cursor position (that is, the position the next character typed would occupy).</dd>
 <dt>{{htmlattrdef("size")}}</dt>
 <dd>The initial size of the control. This value is in pixels unless the value of the <strong>type</strong> attribute is <code>text</code> or <code>password</code>, in which case it is an integer number of characters. Starting in HTML5, this attribute applies only when the <strong>type</strong> attribute is set to <code>text</code>, <code>search</code>, <code>tel</code>, <code>url</code>, <code>email</code>, or <code>password</code>, otherwise it is ignored. In addition, the size must be greater than zero. If you do not specify a size, a default value of 20 is used. HTML5 simply states "the user agent should ensure that at least that many characters are visible", but different characters can have different widths in certain fonts. In some browsers, a certain string with <em>x</em> characters will not be entirely visible even if size is defined to at least <em>x</em>.</dd>
 <dt>{{htmlattrdef("spellcheck")}}</dt>
 <dd>Setting the value of this attribute to <code>true</code> indicates that the element needs to have its spelling and grammar checked. The value <code>default</code> indicates that the element is to act according to a default behavior, possibly based on the parent element's own <code>spellcheck</code> value. The value <code>false</code> indicates that the element should not be checked.</dd>
 <dt>{{htmlattrdef("src")}}</dt>
 <dd>If the value of the <strong>type</strong> attribute is <code>image</code>, this attribute specifies a URI for the location of an image to display on the graphical submit button, otherwise it is ignored.</dd>
 <dt>{{htmlattrdef("step")}}</dt>
 <dd>Works with the <strong>min</strong> and <strong>max</strong> attributes to limit the increments at which a numeric or date-time value can be set. It can be the string <code>any</code> or a positive floating point number. If this attribute is not set to <code>any</code>, the control accepts only values at multiples of the step value greater than the minimum.</dd>
 <dt>{{htmlattrdef("tabindex")}}</dt>
 <dd>The position of the element in the tabbing navigation order for the current document.</dd>
 <dt>{{htmlattrdef("usemap")}} {{Deprecated_Inline}}</dt>
 <dd>The name of a {{HTMLElement("map")}} element to be used as an image map.</dd>
 <dt>{{htmlattrdef("value")}}</dt>
 <dd>The initial value of the control. This attribute is optional except when the value of the <strong>type</strong> attribute is <code>radio</code> or <code>checkbox</code>.<br>
 Note that when reloading the page, Gecko and IE <a href="https://bugzilla.mozilla.org/show_bug.cgi?id=46845#c186">will ignore the value specified in the HTML source</a>, if the value was changed before the reload.</dd>
 <dt>{{htmlattrdef("width")}}</dt>
 <dd>If the value of the <strong>type</strong> attribute is <code>image</code>, this attribute defines the width of the image displayed for the button.</dd>
</dl>

<h3 id="Non-standard_&lt;input>_attributes">Non-standard <code>&lt;input&gt;</code> attributes</h3>

<dl>
 <dt>{{htmlattrdef("autocapitalize")}} {{non-standard_inline}}</dt>
 <dd>This is a nonstandard attribute used <a href="https://developers.google.com/web/updates/2015/04/autocapitalize">by Chrome</a> and iOS Safari Mobile, which controls whether and how the text value should be automatically capitalized as it is entered/edited by the user. The non-deprecated values are available in iOS 5 and later. Possible values are:
 <ul>
  <li><code>none</code>: Completely disables automatic capitalisation.</li>
  <li><code>sentences</code>: Automatically capitalise the first letter of sentences.</li>
  <li><code>words</code>: Automatically capitalise the first letter of words.</li>
  <li><code>characters</code>: Automatically capitalise all characters.</li>
  <li><code>on</code>: {{deprecated_inline}} Deprecated since iOS 5.</li>
  <li><code>off</code>: {{deprecated_inline}} Deprecated since iOS 5.</li>
 </ul>
 <a href="https://developer.apple.com/library/safari/documentation/AppleApplications/Reference/SafariHTMLRef/Articles/Attributes.html#//apple_ref/doc/uid/TP40008058-autocapitalize"><code>autocapitalize</code> documentation</a> in the Safari HTML Reference.</dd>
 <dt>{{htmlattrdef("autocorrect")}} {{non-standard_inline}}</dt>
 <dd>This is a non-standard attribute supported by Safari that is used to control whether autocorrection should be enabled when the user is entering/editing the text value of the <code>&lt;input&gt;</code>. Possible attribute values are:
 <ul>
  <li><code>on</code>: Enable autocorrection.</li>
  <li><code>off</code>: Disable autocorrection.</li>
 </ul>
 <a href="https://developer.apple.com/library/safari/documentation/AppleApplications/Reference/SafariHTMLRef/Articles/Attributes.html#//apple_ref/doc/uid/TP40008058-autocorrect"><code>autocorrect</code> documentation</a> in the Safari HTML Reference.</dd>
 <dt>{{htmlattrdef("incremental")}} {{non-standard_inline}}</dt>
 <dd>This is a nonstandard attribute supported by WebKit (Safari) and Blink (Chrome) that only applies when the <strong>type</strong> is <code>search</code>. If the attribute is present, regardless of what its value is, the <code>&lt;input&gt;</code> fires <a href="/en-US/docs/Web/Events/search"><code>search</code></a> events as the user edits the text value. The event is only fired after an implementation-defined timeout has elapsed since the most recent keystroke, and new keystrokes reset the timeout. In other words, the event firing is debounced. If the attribute is absent, the <a href="/en-US/docs/Web/Events/search"><code>search</code></a> event is only fired when the user explicitly initiates a search (e.g. by pressing the Enter key while within field). <a href="https://developer.apple.com/library/safari/documentation/AppleApplications/Reference/SafariHTMLRef/Articles/Attributes.html#//apple_ref/doc/uid/TP40008058-incremental"><code>incremental</code> documentation in the Safari HTML Reference</a></dd>
 <dt>{{htmlattrdef("mozactionhint")}} {{non-standard_inline}}</dt>
 <dd>Specifies an "action hint" used to determine how to label the enter key on mobile devices with virtual keyboards. Supported values are <code>go</code>, <code>done</code>, <code>next</code>, <code>search</code>, and <code>send</code>. These automatically get mapped to the appropriate string and are case-insensitive.</dd>
 <dt>{{htmlattrdef("results")}} {{non-standard_inline}}</dt>
 <dd>This is a nonstandard attribute supported by Safari that only applies when the <strong>type</strong> is <code>search</code>. It is used to control the maximum number of entries that should be displayed in the <code>&lt;input&gt;</code>'s native dropdown list of past search queries. Its value should be a nonnegative decimal integer.</dd>
 <dt>{{htmlattrdef("webkitdirectory")}} {{non-standard_inline}}</dt>
 <dd>This Boolean attribute indicates if the selector used when the <strong>type</strong> attribute is <code>file</code> has to allow for the selection of directories only.</dd>
 <dt>{{htmlattrdef("x-moz-errormessage")}} {{non-standard_inline}}</dt>
 <dd>This Mozilla extension allows you to specify the error message to display when a field doesn't successfully validate.</dd>
</dl>

<h2 id="Examples">Examples</h2>

<p>You can find multiple examples of <code>&lt;input&gt;</code> element usage on the pages covering each individual type — see <a href="#form_&lt;input>_types">Form &lt;input&gt; types</a>, and also see the <a href="#live_example">Live example</a> at the top of the article.</p>

<ul>
</ul>

<h2 id="Specifications">Specifications</h2>

{{Specifications}}

<h2 id="Browser_compatibility">Browser compatibility</h2>

{{Compat("html.elements.input")}}

<h2 id="Notes">Notes</h2>

<h3 id="File_inputs">File inputs</h3>

<ol>
 <li>
  <p>Starting in {{Gecko("2.0")}}, calling the <code>click()</code> method on an <code>&lt;input&gt;</code> element of type <code>file</code> opens the file picker and lets the user select files. See <a href="/en-US/docs/Using_files_from_web_applications">Using files from web applications</a> for an example and more details.</p>
 </li>
 <li>
  <p>You cannot set the value of a file picker from a script — doing something like the following has no effect:</p>

  <pre class="brush: js">var e = getElementById("someFileInputElement");
e.value = "foo";
</pre>
 </li>
 <li>
  <p>When a file is chosen using an <code>&lt;input type="file"&gt;</code>, the real path to the source file is not shown in the input's <code>value</code> attribute for obvious security reasons. Instead, the filename is shown, with <code>C:\fakepath\</code> appended to the beginning of it. There are some historical reasons for this quirk, but it is supported across all modern browsers, and in fact is <a href="https://html.spec.whatwg.org/multipage/forms.html#fakepath-srsly">defined in the spec</a>.</p>
 </li>
</ol>

<h3 id="Error_messages">Error messages</h3>

<p>If you want Firefox to present a custom error message when a field fails to validate, you can use the <code>x-moz-errormessage</code> attribute to do so:</p>

<pre class="brush: html">&lt;input type="email"
 x-moz-errormessage="Please specify a valid email address."&gt;
</pre>

<p>Note, however, that this is not standard and will not have an effect on other browsers.</p>

<h3 id="Localization">Localization</h3>

<p>The allowed inputs for certain &lt;input&gt; types depend on the locale. In some locales, 1,000.00 is a valid number, while in other locales the valid way to enter this number is 1.000,00.</p>

<p>Firefox uses the following heuristics to determine the locale to validate the user's input (at least for <code>type="number"</code>):</p>

<ul>
 <li>Try the language specified by a <code>lang</code>/<code>xml:lang</code> attribute on the element or any of its parents.</li>
 <li>Try the language specified by any Content-Language HTTP header or</li>
 <li>If none specified, use the browser's locale.</li>
</ul>

<h3 id="Using_mozactionhint_on_Firefox_mobile">Using mozactionhint on Firefox mobile</h3>

<p>You can use the {{htmlattrxref("mozactionhint", "input")}} attribute to specify the text for the label of the enter key on the virtual keyboard when your form is rendered on Firefox mobile. For example, to have a "Next" label, you can do this:</p>

<pre class="brush: html">&lt;input type="text" mozactionhint="next"&gt;
</pre>

<p>The result is:</p>

<p><img alt="mozactionhint.png" src="/@api/deki/files/4970/=mozactionhint.png?size=webview"></p>

<h2 id="See_also">See also</h2>

<ul>
 <li>Other form-related elements: {{HTMLElement("form")}}, {{HTMLElement("button")}}, {{HTMLElement("datalist")}}, {{HTMLElement("legend")}}, {{HTMLElement("label")}}, {{HTMLElement("select")}}, {{HTMLElement("optgroup")}}, {{HTMLElement("option")}}, {{HTMLElement("textarea")}}, {{HTMLElement("keygen")}}, {{HTMLElement("fieldset")}}, {{HTMLElement("output")}}, {{HTMLElement("progress")}} and {{HTMLElement("meter")}}.</li>
 <li><a href="http://webdesignerwall.com/tutorials/cross-browser-html5-placeholder-text">Cross-browser HTML5 placeholder text</a></li>
</ul>
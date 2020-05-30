---
title: How we use Cloudflare image resizing at MasterClass
date: 2020-05-30T19:12:08.751Z
thumbnail: assets/operahaus-top.jpg
---
<main class="wysiwyg">
      <p>
        <code><a href="https://github.com/jgthms/wysiwyg.css">wysiwyg.css</a></code> file is a simple <strong>collection of styles</strong> targeted at HTML elements generated from a <abbr title="What You See Is What You Get">WYSIWYG</abbr> editor (like TinyMCE) or Markdown.
      </p>
      <p>
        Its purpose are:
      </p>
      <ul>
        <li>
          <strong>readability</strong>: both the spacing and colors are visually <em>balanced</em>
        </li>
        <li>
          <strong>simplicity</strong>: you only need a <em>single</em> class to style all elements
        </li>
        <li>
          <strong>extensibility</strong>: you can easily <em>customise</em> the output thanks to variables
        </li>
      </ul>
      <p>
        As a matter of fact, <code>wysiwyg.css</code> supports <a href="https://github.com/jgthms/wysiwyg.css/blob/master/themes">themes</a>.
      </p>
      <h2>Example</h2>
      <p>
        This whole white block of content only uses a single CSS class on its container.
        <br>
        Everything inside are HTML elements with no additional class.
      </p>
      <h2>How it works</h2>
      <p>
        You just add the <code>.wysiwyg</code> CSS class to a <strong>container</strong>, and it will style all its child elements:
      </p>
<pre>&lt;div class="wysiwyg"&gt;
  &lt;!-- Your generated HTML --&gt;
&lt;/div&gt;
</pre>
      <p>
        In order to blend in gracefully with your design, the <code>wysiwyg</code> container will <strong>inherit colors</strong> (for text, headings and links) and <strong>typography</strong> (font family, size and smoothing).
      </p>
      <h2>What it styles</h2>
      <h3>Blocks</h3>
      <ul>
        <li>Headings: from <code>&lt;h1&gt;</code> to <code>&lt;h6&gt;</code></li>
        <li>Paragraphs <code>&lt;p&gt;</code></li>
        <li>Lists: <code>&lt;ol&gt;</code> and <code>&lt;ul&gt;</code></li>
        <li>Blockquotes <code>&lt;blockquote&gt;</code></li>
        <li>Tables <code>&lt;table&gt;</code> <code>&lt;tr&gt;</code> <code>&lt;th&gt;</code> and <code>&lt;td&gt;</code></li>
        <li>Pre <code>&lt;pre&gt;</code></li>
        <li>Figures <code>&lt;figure&gt;</code> and <code>&lt;figcaption&gt;</code></li>
      </ul>
      <h3>Inline elements</h3>
      <ul>
        <li>
          Links:
          <code>&lt;a&gt;</code>
        </li>
        <li>
          Semantic:
          <code>&lt;strong&gt;</code>
          and
          <code>&lt;em&gt;</code>
        </li>
        <li>
          Code:
          <code>&lt;code&gt;</code>
          <code>&lt;kbd&gt;</code>
          and
          <code>&lt;samp&gt;</code>
        </li>
        <li>
          Abbreviations:
          <code>&lt;abbr&gt;</code>
          </li>
        <li>
          Notations:
          <code>&lt;mark&gt;</code>
          <code>&lt;s&gt;</code>
          <code>&lt;del&gt;</code>
          and
          <code>&lt;ins&gt;</code>
        </li>
        <li>
          Quotes:
          <code>&lt;q&gt;</code>
          and
          <code>&lt;cite&gt;</code>
        </li>
        <li>
          Other:
          <code>&lt;small&gt;</code>
          <code>&lt;sub&gt;</code>
          <code>&lt;sup&gt;</code>
          <code>&lt;hr&gt;</code>
        </li>
      </ul>
      <h2>How it looks</h2>
      <p>
        The content you're reading is styled using <code>wysiwyg.css</code> with its default parameters.
      </p>
      <p>
        You can have paragraphs,
        with <a href="#">links</a>,
        <strong>important</strong> or <em>emphasised</em> words,
        <code>code snippets</code>,
        <abbr title="abbreviations">abbr</abbr>,
        <q>short quotes</q>,
        <cite>citations</cite>,
        <mark>highlighted text</mark>,
        <kbd>keyboard inputs</kbd>,
        <s>strikethrough</s>,
        <del>deleted</del> and <ins>inserted</ins> elements,
        <samp>sample text</samp>,
        <small>small text</small>,
        and
        words with<sub>sub</sub>and<sup>sup</sup>text.
      </p>
      <p>
        You also have horizontal breaks.
      </p>
      <hr>
      <p>You also have <strong>unordered lists</strong>:</p>
      <ul>
        <li>
          From basic lists
          <ul>
            <li>
              With nested items
              <ul>
                <li>
                  That have a different bullet point
                  <ul>
                    <li>
                      At each level
                      <ul>
                        <li>
                          Up to
                          <ul>
                            <li>The 6th level</li>
                          </ul>
                        </li>
                      </ul>
                    </li>
                  </ul>
                </li>
              </ul>
            </li>
          </ul>
        </li>
        <li>With items that can spawn multiple lines</li>
        <li>Like this one: lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas at aliquet orci. Curabitur eget porttitor sem. Aenean eu convallis diam. Sed nibh massa, rhoncus id interdum pellentesque, congue ac erat.</li>
      </ul>
      <p>
        And <strong>ordered lists</strong>:
      </p>
      <ol>
        <li>
          Step one
          <ol>
            <li>
              Side step one
              <ol>
                <li>
                  Side step two
                  <ol>
                    <li>
                      Site step three
                      <ol>
                        <li>
                          Side step four
                          <ol>
                            <li>Side step five</li>
                          </ol>
                        </li>
                      </ol>
                    </li>
                  </ol>
                </li>
              </ol>
            </li>
          </ol>
        </li>
        <li>Step two</li>
        <li>????</li>
        <li>PROFIT!!!</li>
      </ol>
      <p>
        And even <strong>definition lists</strong>:
      </p>
      <dl>
        <dt>Name</dt>
        <dd>Godzilla</dd>
        <dt>Born</dt>
        <dd>1952</dd>
        <dt>Birthplace</dt>
        <dd>Japan</dd>
        <dt>Color</dt>
        <dd>Green</dd>
      </dl>
      <blockquote>
        You can also use the <code>blockquote</code> element.
        It can be used with or without paragraphs.
      </blockquote>
      <p>
        The <strong>figure</strong> and related <em>figcaption</em> elements are supported:
      </p>
      <figure>
        <a href="https://jgthms.com/web-design-in-4-minutes/">
          <img src="https://jgthms.com/web-design-in-4-minutes/web-design-in-4-minutes.png" alt="Web design in 4 minutes" width="1200" height="630">
        </a>
        <figcaption>A full width image</figcaption>
      </figure>
      <figure>
        <img src="https://developer.cdn.mozilla.net/media/img/mdn-logo-sm.png" alt="An awesome picture" width="62" height="71">
        <figcaption>A small image</figcaption>
      </figure>
      <p>
        <strong>Tables</strong> are supported: cells, rows, head, body, and foot are styled.
      </p>
      <table>
        <thead>
          <tr>
            <th>Name</th>
            <th>Instruments</th>
            <th>Period</th>
          </tr>
        </thead>
        <tfoot>
          <tr>
            <th>Name</th>
            <th>Instruments</th>
            <th>Period</th>
          </tr>
        </tfoot>
        <tbody>
          <tr>
            <td>John Lennon</td>
            <td>Vocals, Guitar</td>
            <td>1960–1969</td>
          </tr>
          <tr>
            <td>Paul McCartney</td>
            <td>Vocals, Bass Guitar</td>
            <td>1960–1970</td>
          </tr>
          <tr>
            <td>George Harrison</td>
            <td>Guitar</td>
            <td>1960–1970</td>
          </tr>
          <tr>
            <td>Ringo Starr</td>
            <td>Drums</td>
            <td>1962–1970</td>
          </tr>
        </tbody>
      </table>
      <h2>Customisation</h2>
      <p>
        To provide flexibility, <code>wysiwyg.css</code> is written in <a href="https://sass-lang.com">Sass</a> and comes with a list of <strong>variables</strong> and <strong>options.</strong>
      </p>
      <h3>Variables</h3>
      <table>
        <thead>
          <tr>
            <th>Name</th>
            <th>Default value</th>
          </tr>
        </thead>
        <tbody>
          <tr><th colspan="2">Colours</th></tr>
          <tr><td><code>$blue</code></td><td><code>#2478ff</code></td></tr>
          <tr><td><code>$pink</code></td><td><code>#ff2450</code></td></tr>
          <tr><td><code>$purple</code></td><td><code>#9524ff</code></td></tr>
          <tr><td><code>$grey-light</code></td><td><code>hsl(0, 0%, 50%)</code></td></tr>
          <tr><td><code>$grey</code></td><td><code>hsl(0, 0%, 20%)</code></td></tr>
          <tr><td><code>$grey-dark</code></td><td><code>hsl(0, 0%, 10%)</code></td></tr>
          <tr><td><code>$background</code></td><td><code>hsl(0, 0%, 95%)</code></td></tr>
          <tr><td><code>$border</code></td><td><code>hsl(0, 0%, 90%)</code></td></tr>
          <tr><td><code>$text</code></td><td><code>$grey</code></td></tr>
          <tr><td><code>$text-code</code></td><td><code>$pink</code></td></tr>
          <tr><td><code>$text-strong</code></td><td><code>$grey-dark</code></td></tr>
          <tr><td><code>$text-light</code></td><td><code>$grey-light</code></td></tr>
          <tr><td><code>$text-headings</code></td><td><code>$grey-dark</code></td></tr>
          <tr><td><code>$text-blockquote</code></td><td><code>$grey-light</code></td></tr>
          <tr><td><code>$link</code></td><td><code>$blue</code></td></tr>
          <tr><td><code>$link-hover</code></td><td><code>$blue</code></td></tr>
          <tr><td><code>$link-visited</code></td><td><code>$purple</code></td></tr>
          <tr><td><code>$background-code</code></td><td><code>$background</code></td></tr>
          <tr><td><code>$background-ins</code></td><td><code>lime</code></td></tr>
          <tr><td><code>$background-mark</code></td><td><code>yellow</code></td></tr>
          <tr><td><code>$table-background</code></td><td><code>hsl(0, 0%, 100%)</code></td></tr>
          <tr><td><code>$table-background-even</code></td><td><code>hsl(0, 0%, 98%)</code></td></tr>
          <tr><td><code>$table-background-hover</code></td><td><code>hsl(0, 0%, 96%)</code></td></tr>
          <tr><td><code>$table-border</code></td><td><code>$border</code></td></tr>
          <tr><td><code>$table-thead</code></td><td><code>$grey-dark</code></td></tr>
          <tr><th colspan="2">Spacing</th></tr>
          <tr><td><code>$line-height</code></td><td><code>1.6</code></td></tr>
          <tr><td><code>$margin</code></td><td><code>1.4em</code></td></tr>
          <tr><th colspan="2">Typography</th></tr>
          <tr><td><code>$family-wysiwyg</code></td><td><pre>-apple-system, BlinkMacSystemFont, "Segoe UI", "Roboto", "Oxygen", "Ubuntu", "Cantarell", "Fira Sans", "Droid Sans", "Helvetica Neue", "Helvetica", "Arial", sans-serif</pre></td></tr>
          <tr><td><code>$family-code</code></td><td><pre>"Inconsolata", "Consolas", "Monaco", monospace</pre></td></tr>
          <tr><td><code>$weight-strong</code></td><td><code>700</code></td></tr>
          <tr><td><code>$weight-headings</code></td><td><code>700</code></td></tr>
        </tbody>
      </table>
      <h3>Options</h3>
      <p>
        By <strong>default</strong>, all options are set to <code>false</code>.
      </p>
      <table>
        <thead>
          <tr>
            <th>Option</th>
            <th>If set to <code>true</code></th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>
              <code>$closer-lists</code>
            </td>
            <td>
              <p>Brings <strong>lists</strong> closer to the <strong>paragraph</strong> they <em>immediately</em> follow</p>
            </td>
          </tr>
          <tr>
            <td>
              <code>$custom-colors</code>
            </td>
            <td>
              <p>Applies the <strong>color</strong> variables to the content:</p>
              <ul>
                <li><code>$text</code></li>
                <li><code>$link</code></li>
                <li><code>$text-strong</code></li>
                <li><code>$text-headings</code></li>
                <li><code>$text-blockquote</code></li>
                <li><code>$text-code</code></li>
                <li><code>$text-light</code></li>
                <li><code>$table-thead</code></li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>
              <code>$custom-fonts</code>
            </td>
            <td>
              <p>Applies the <strong>font-family</strong> variables to the content:</p>
              <ul>
                <li><code>$family-wysiwyg</code></li>
                <li><code>$family-code</code></li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>
              <code>$font-smoothing</code>
            </td>
            <td>
              <p>Applies <a href="https://developer.mozilla.org/en-US/docs/Web/CSS/font-smooth">font smoothing</a> to non-code content</p>
            </td>
          </tr>
          <tr>
            <td>
              <code>$heading-borders</code>
            </td>
            <td>
              <p>Adds <strong>bottom borders</strong> to <code>h1</code> and <code>h2</code></p>
            </td>
          </tr>
          <tr>
            <td>
              <code>$show-underline</code>
            </td>
            <td>
              <p><strong>Underlines</strong> links</p>
            </td>
          </tr>
          <tr>
            <td>
              <code>$striped-rows</code>
            </td>
            <td>
              <p>Adds striped rows to <strong>tables</strong></p>
            </td>
          </tr>
          <tr>
            <td>
              <code>$visited-links</code>
            </td>
            <td>
              <p>Applies the <code>$link-visited</code> color to <strong>visited links</strong></p>
            </td>
          </tr>
        </tbody>
      </table>
    </main>
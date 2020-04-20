# WCAG Checklist \(Work-in-Progress\)

Section 508 Compliance references WCAG 2.0 Level A and Level AA Success Criteria and Conformance Requirements. WCAG 2.0 is the standard teams have used since January of 2017. In 2019, WCAG 2.1 was released and is expected to become the standard for compliance. This checklist below offers organized guidance to meet Section 508 Compliance. Another reference that may be useful is [How to Meet WCAG, Quick Reference](https://www.w3.org/WAI/WCAG21/quickref/).

Note: Based on WCAG 2.0 AA Requirements \(marked with “MUST”\) and best practices \(marked with “_SHOULD_”\) _\(Based on_ [https://www.jenstrickland.design/talks/design4performance-a11y/resources/WCAG\_Checklist.pdf](https://www.jenstrickland.design/talks/design4performance-a11y/resources/WCAG_Checklist.pdf)_\)_

## Part 1: Semantic Structure

_Rebuilding the table in HTML to use rowspan_

<table>
  <thead>
    <tr>
      <th style="text-align:left">Topic</th>
      <th style="text-align:left">Accessibility Requirements</th>
      <th style="text-align:left">WCAG</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Page title</td>
      <td style="text-align:left">
        <p> <b>The page MUST have a meaningful title</b> (e.g. About us), even when
          included via iframe.</p>
        <ul>
          <li>Unique information *SHOULD* go first (e.g. &#x201C;WCAG Checklist&#x201D;).</li>
          <li>Result pages <em>SHOULD</em> describe the result (e.g. &#x201C;Error on
            form&#x201D; or &#x201C;Search results loaded&#x201D;).</li>
          <li>Single-page applications and AJAX scripts <em>SHOULD</em> update the title
            when the URL changes or, when the page content changes significantly.</li>
        </ul>
      </td>
      <td style="text-align:left"> <a href="https://www.w3.org/WAI/WCAG21/Understanding/page-titled.html">2.4.2</a>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Language</td>
      <td style="text-align:left"> <b>The page MUST specify the language</b> (&lt;html lang=&quot;en&quot;&gt;).</td>
      <td
      style="text-align:left"> <a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/meaning-doc-lang-id.html">3.1.1</a>
        </td>
    </tr>
    <tr>
      <td style="text-align:left"> <b>Changes in the language within the page MUST be specified</b> (e.g.
        &lt;span lang=&quot;es&quot;&gt;Hola&lt;/span&gt;).</td>
      <td style="text-align:left"> <a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/meaning-other-lang-id.html">3.1.2</a>
      </td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">Landmarks</td>
      <td style="text-align:left"> <b>Pages </b><em><b>SHOULD</b></em><b> have accurate, logical landmark structure</b> (e.g.
        &lt;header&gt;, &lt;nav&gt;, &lt;main&gt;, &lt;aside&gt;, &lt;footer&gt;),
        so screen reader users can navigate by landmark, and all content SHOULD
        be inside a landmark.</td>
      <td style="text-align:left"> <a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-descriptive.html">2.4.6</a>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Headings</td>
      <td style="text-align:left"> <b>The page MUST have meaningful headings to label each major section</b>,
        which <em>SHOULD</em> start with &lt;h1&gt; (at the beginning of the main
        content, or at the beginning of every section of aggregated content, or
        at the beginning of modal dialogs), and <em>SHOULD NOT</em> skip heading
        levels, to allow screen reader users to navigate the tree structure of
        the heading hierarchy.</td>
      <td style="text-align:left"> <a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-descriptive.html">2.4.6</a>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>Links and Navigation
          <br />
        </p>
        <p>(See also Custom Widgets in Part 3 for dynamic menus (drop-down accordion,
          etc.)</p>
      </td>
      <td style="text-align:left"> <b>Links MUST have readable text</b>. Be especially careful with links
        that contain only images (which need alt text) and background images/icon
        fonts (which need text via aria-label on the link or text within the link,
        hidden via CSS).</td>
      <td style="text-align:left"> <a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/ensure-compat-rsv.html">4.1.2</a>,
        <a
        href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-link.html">2.4.9</a>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"> <b>The link text MUST make sense in context, and should make sense when taken out of context</b> (problematic
        phrases include: &#x201C;click here,&#x201D; &#x201C;learn more,&#x201D;
        &#x201C;more,&#x201D; &#x201C;read more,&#x201D; etc.).</td>
      <td style="text-align:left"> <a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-link.html">2.4.9</a>,
        <a
        href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-refs.html">2.4.4</a>
      </td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"> <b>Linked content SHOULD be grouped in a single link where appropriate</b>.
        For example: an icon and its adjacent text SHOULD NOT be two separate links
        if they go to the same location.</td>
      <td style="text-align:left"> <a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/consistent-behavior-consistent-functionality.html">3.2.4</a>
      </td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"> <b>Navigation features (e.g. main menu) MUST be placed in a consistent location across pages</b>.</td>
      <td
      style="text-align:left"> <a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/consistent-behavior-consistent-locations.html">3.2.3</a>
        </td>
        <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"> <b>Navigation features MUST be identified in a consistent way across pages</b>.</td>
      <td
      style="text-align:left"> <a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/consistent-behavior-consistent-functionality.html">3.2.4</a>
        </td>
        <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"> <b>A &#x201C;skip navigation&#x201D; or &#x201C;skip to main content&#x201D; SHOULD be provided as the first link in the design</b>,
        to allow sighted keyboard users to quickly arrive at the main content (Note:
        the link can be invisible until the user tabs to it, but it MUST NOT remain
        invisible when it receives keyboard focus).</td>
      <td style="text-align:left"> <a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-mult-loc.html">2.4.5</a>
      </td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">Tables</td>
      <td style="text-align:left"> <b>Header cells (&lt;th&gt;) MUST be associated with their respective data cells</b> (via
        scope or headers + id).</td>
      <td style="text-align:left"> <a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/content-structure-separation-programmatic.html">1.3.1</a>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"> <b>Tables SHOULD have an accessible name</b> (e.g. &lt;caption&gt;, aria-label,
        or aria-labelledby).</td>
      <td style="text-align:left"> <a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/ensure-compat-rsv.html">4.1.2</a>
      </td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"> <b>Layout tables (no header/data associations) MUST NOT contain &lt;th&gt; or other header markup.</b>
      </td>
      <td style="text-align:left"> <a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/content-structure-separation-programmatic.html">1.3.1</a>
      </td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">Lists</td>
      <td style="text-align:left"> <b>Lists MUST be marked up appropriately</b> according to the semantics
        of the list (e.g. &lt;ul&gt;, &lt;ol&gt;, &lt;dl&gt;).</td>
      <td style="text-align:left"> <a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/content-structure-separation-programmatic.html">1.3.1</a>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
  </tbody>
</table>| Topic | Accessibility Requirements | WCAG |
| :--- | :--- | :--- |
| **iframes** | **Frame title attribute MUST be specified** \(`<iframe title="Video about..."`\). | 4.1.2 |
| **iframes** | **The page within the iframe MUST have an accurate, meaningful 1`<title>`1.** | 2.4.2 |
| **iframes** | **Iframes with no readable content \(e.g. only JavaScript\) SHOULD be set to aria-hidden="true".** | \(4.1.2\) |
| **Form Markup**   \(See also Form Validation and Feedback in Part 3\) | **Inputs, buttons, and controls MUST have labels which are programmatically-associated** \(e.g. via `<label>`, aria-label, or aria-labelledby\) **and always visible on the screen** \(they don’t disappear when the user starts typing\). | 1.3.1, 3.3.2 |
| **Form Markup**   \(See also Form Validation and Feedback in Part 3\) | **Required fields SHOULD be marked as such**, e.g. via aria-required="true" \(on the input, not on the label\), or have the word “required” in the `<label>` text. | 3.3.2 |
| **Form Markup**   \(See also Form Validation and Feedback in Part 3\) | **Form field instructions SHOULD be associated with inputs or buttons** using techniques such as: Putting the instructions in the `<label>`. Associating the instructions with the field using aria-describedby \(Note: text associated via aria-describedby _SHOULD_ be relatively brief\). Putting the instructions in a `<fieldset>` with `<legend>` | 3.3.2 |
| **Form Markup**   \(See also Form Validation and Feedback in Part 3\) | **Groups of form elements MUST have group labels** \(e.g. `<fieldset>` and `<legend>`, or referenced from the inputs via aria-labelledby="id-of-group-label id-of-self-label" \). | 1.3.1 |
| **Parsing and Validity** | **The page MUST NOT contain duplicate IDs** because accessibility features frequently reference IDs. | 4.1.1 |
| **Parsing and Validity** | **Attributes \(e.g. ARIA\) MUST contain only allowable values, in the proper parent-child hierarchy.** | 4.1.1 |
| **Parsing and Validity** | **Parent-child relationships of elements & attributes \(e.g. ARIA roles\) MUST follow the specification.** | 4.1.1 |
| **Parsing and Validity** | **The page MUST NOT contain syntax errors that affect semantic meaning** \(e.g. elements or attributes that don’t close properly, either explicitly or implicitly\). | 4.1.1 |

## Part 2: Sight & Sound

| Topic | Accessibility Requirements | WCAG |
| :--- | :--- | :--- |
| Heading |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |

| Topic | Accessibility Requirements | WCAG |
| :--- | :--- | :--- |
| **Word** | Word | Numbers |
| **Word** | Word | Numbers |
| **Word** | Word | Numbers |
| **Word** | Word | Numbers |
| **Word** | Word | Numbers |
| **Word** | Word | Numbers |
| **Word** | Word | Numbers |
| **Word** | Word | Numbers |
| **Word** | Word | Numbers |
| **Word** | Word | Numbers |
| **Word** | Word | Numbers |
| **Word** | Word | Numbers |


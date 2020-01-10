.. include:: ../Includes.txt


.. _typoscript-syntax-typoscript-templates-usage:

Usage
=====

TypoScript templates are used to drive frontend rendering.

TYPO3 CMS does not provide a definite templating method out of the box.
However a minimal amount of TypoScript will *always* be necessary to
tell TYPO3 CMS which templating method to use.
It could be any of the following:

- **Fluid templates:** Configure TYPO3 to use Extbase and Fluid
  for templating. This allows to use external HTML templates, but
  with fluid-style variables with curly braces. A content object
  :ref:`cobj-fluidtemplate` is available, which uses Fluid
  from inside TypoScript.

- **HTML templates:** Configure TYPO3 CMS to facilitate external HTML-
  templates with markers and subparts. Please see the :ref:`Templating Tutorial <t3templating:start>`.

- **External Templating Engines:** Any other templating system can be
  used. It will be provided via an extension. In such a case TypoScript
  may be used just to delegate the rendering to that system.

- **Custom PHP:** Configure TYPO3 to call your own PHP code which
  generates content in any way you may prefer. This might include using
  third party templating engines!

- **TS content objects:** Build the page entirely using TypoScript
  content objects. All these objects are highly configurable.

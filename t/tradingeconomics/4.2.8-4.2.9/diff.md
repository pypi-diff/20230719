# Comparing `tmp/tradingeconomics-4.2.8.tar.gz` & `tmp/tradingeconomics-4.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradingeconomics-4.2.8.tar", last modified: Tue Jul 11 18:23:49 2023, max compression
+gzip compressed data, was "tradingeconomics-4.2.9.tar", last modified: Wed Jul 19 15:34:01 2023, max compression
```

## Comparing `tradingeconomics-4.2.8.tar` & `tradingeconomics-4.2.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:23:49.623940 tradingeconomics-4.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-11 18:23:35.000000 tradingeconomics-4.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 18:23:35.000000 tradingeconomics-4.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-11 18:23:49.623940 tradingeconomics-4.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-11 18:23:35.000000 tradingeconomics-4.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 18:23:49.623940 tradingeconomics-4.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-11 18:23:35.000000 tradingeconomics-4.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:23:49.619940 tradingeconomics-4.2.8/tradingeconomics/
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-11 18:23:35.000000 tradingeconomics-4.2.8/tradingeconomics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-07-11 18:23:35.000000 tradingeconomics-4.2.8/tradingeconomics/calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    16086 2023-07-11 18:23:35.000000 tradingeconomics-4.2.8/tradingeconomics/comtrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-07-11 18:23:35.000000 tradingeconomics-4.2.8/tradingeconomics/earnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-07-11 18:23:35.000000 tradingeconomics-4.2.8/tradingeconomics/eurostat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-07-11 18:23:35.000000 tradingeconomics-4.2.8/tradingeconomics/federalReserve.py
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-07-11 18:23:35.000000 tradingeconomics-4.2.8/tradingeconomics/financials.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-11 18:23:35.000000 tradingeconomics-4.2.8/tradingeconomics/forecasts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-07-11 18:23:35.000000 tradingeconomics-4.2.8/tradingeconomics/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-11 18:23:35.000000 tradingeconomics-4.2.8/tradingeconomics/glob.py
--rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-07-11 18:23:35.000000 tradingeconomics-4.2.8/tradingeconomics/historical.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-11 18:23:35.000000 tradingeconomics-4.2.8/tradingeconomics/historicalDB.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-11 18:23:35.000000 tradingeconomics-4.2.8/tradingeconomics/historicalEurostat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-11 18:23:35.000000 tradingeconomics-4.2.8/tradingeconomics/historicalFinancials.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-11 18:23:35.000000 tradingeconomics-4.2.8/tradingeconomics/historicalMarkets.py
--rw-r--r--   0 runner    (1001) docker     (123)    15800 2023-07-11 18:23:35.000000 tradingeconomics-4.2.8/tradingeconomics/indicators.py
--rw-r--r--   0 runner    (1001) docker     (123)    21590 2023-07-11 18:23:35.000000 tradingeconomics-4.2.8/tradingeconomics/markets.py
--rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-07-11 18:23:35.000000 tradingeconomics-4.2.8/tradingeconomics/news.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-11 18:23:35.000000 tradingeconomics-4.2.8/tradingeconomics/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-11 18:23:35.000000 tradingeconomics-4.2.8/tradingeconomics/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-11 18:23:35.000000 tradingeconomics-4.2.8/tradingeconomics/worldBank.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:23:49.623940 tradingeconomics-4.2.8/tradingeconomics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-11 18:23:49.000000 tradingeconomics-4.2.8/tradingeconomics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-11 18:23:49.000000 tradingeconomics-4.2.8/tradingeconomics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 18:23:49.000000 tradingeconomics-4.2.8/tradingeconomics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-11 18:23:49.000000 tradingeconomics-4.2.8/tradingeconomics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 18:23:49.000000 tradingeconomics-4.2.8/tradingeconomics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 15:34:01.696124 tradingeconomics-4.2.9/
+-rw-rw-rw-   0        0        0    35823 2023-07-10 13:38:05.000000 tradingeconomics-4.2.9/LICENSE
+-rw-rw-rw-   0        0        0       18 2023-07-10 13:38:05.000000 tradingeconomics-4.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2401 2023-07-19 15:34:01.696124 tradingeconomics-4.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1708 2023-07-10 13:38:05.000000 tradingeconomics-4.2.9/README.rst
+-rw-rw-rw-   0        0        0       86 2023-07-19 15:34:01.700394 tradingeconomics-4.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1157 2023-07-19 15:33:47.000000 tradingeconomics-4.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:34:01.666012 tradingeconomics-4.2.9/tradingeconomics/
+-rw-rw-rw-   0        0        0     3639 2023-07-10 13:38:05.000000 tradingeconomics-4.2.9/tradingeconomics/__init__.py
+-rw-rw-rw-   0        0        0    11093 2023-07-11 18:45:19.000000 tradingeconomics-4.2.9/tradingeconomics/calendar.py
+-rw-rw-rw-   0        0        0    16441 2023-07-18 14:46:49.000000 tradingeconomics-4.2.9/tradingeconomics/comtrade.py
+-rw-rw-rw-   0        0        0     4395 2023-07-10 13:38:05.000000 tradingeconomics-4.2.9/tradingeconomics/earnings.py
+-rw-rw-rw-   0        0        0     7002 2023-07-10 13:38:05.000000 tradingeconomics-4.2.9/tradingeconomics/eurostat.py
+-rw-rw-rw-   0        0        0    12372 2023-07-10 13:38:05.000000 tradingeconomics-4.2.9/tradingeconomics/federalReserve.py
+-rw-rw-rw-   0        0        0     6398 2023-07-10 13:38:05.000000 tradingeconomics-4.2.9/tradingeconomics/financials.py
+-rw-rw-rw-   0        0        0     5244 2023-07-10 13:38:05.000000 tradingeconomics-4.2.9/tradingeconomics/forecasts.py
+-rw-rw-rw-   0        0        0     8933 2023-07-10 13:38:05.000000 tradingeconomics-4.2.9/tradingeconomics/functions.py
+-rw-rw-rw-   0        0        0     1234 2023-07-10 13:38:05.000000 tradingeconomics-4.2.9/tradingeconomics/glob.py
+-rw-rw-rw-   0        0        0    13237 2023-07-10 13:38:05.000000 tradingeconomics-4.2.9/tradingeconomics/historical.py
+-rw-rw-rw-   0        0        0     4509 2023-07-10 13:38:05.000000 tradingeconomics-4.2.9/tradingeconomics/historicalDB.py
+-rw-rw-rw-   0        0        0     3073 2023-07-10 13:38:05.000000 tradingeconomics-4.2.9/tradingeconomics/historicalEurostat.py
+-rw-rw-rw-   0        0        0     2702 2023-07-10 13:38:05.000000 tradingeconomics-4.2.9/tradingeconomics/historicalFinancials.py
+-rw-rw-rw-   0        0        0     4185 2023-07-10 13:38:05.000000 tradingeconomics-4.2.9/tradingeconomics/historicalMarkets.py
+-rw-rw-rw-   0        0        0    16263 2023-07-10 13:38:05.000000 tradingeconomics-4.2.9/tradingeconomics/indicators.py
+-rw-rw-rw-   0        0        0    22652 2023-07-18 14:46:49.000000 tradingeconomics-4.2.9/tradingeconomics/markets.py
+-rw-rw-rw-   0        0        0    13802 2023-07-10 13:38:05.000000 tradingeconomics-4.2.9/tradingeconomics/news.py
+-rw-rw-rw-   0        0        0     2243 2023-07-10 13:38:05.000000 tradingeconomics-4.2.9/tradingeconomics/search.py
+-rw-rw-rw-   0        0        0     1969 2023-07-10 13:38:05.000000 tradingeconomics-4.2.9/tradingeconomics/stream.py
+-rw-rw-rw-   0        0        0     9449 2023-07-10 13:38:05.000000 tradingeconomics-4.2.9/tradingeconomics/worldBank.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:34:01.693125 tradingeconomics-4.2.9/tradingeconomics.egg-info/
+-rw-rw-rw-   0        0        0     2401 2023-07-19 15:34:01.000000 tradingeconomics-4.2.9/tradingeconomics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      894 2023-07-19 15:34:01.000000 tradingeconomics-4.2.9/tradingeconomics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 15:34:01.000000 tradingeconomics-4.2.9/tradingeconomics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-19 15:34:01.000000 tradingeconomics-4.2.9/tradingeconomics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-19 15:34:01.000000 tradingeconomics-4.2.9/tradingeconomics.egg-info/top_level.txt
```

### Comparing `tradingeconomics-4.2.8/LICENSE` & `tradingeconomics-4.2.9/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `tradingeconomics-4.2.8/PKG-INFO` & `tradingeconomics-4.2.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-Metadata-Version: 2.1
-Name: tradingeconomics
-Version: 4.2.8
-Summary: Trading Economics API
-Home-page: https://github.com/tradingeconomics/tradingeconomics-python
-Download-URL: https://github.com/tradingeconomics/tradingeconomics-python/tree/main/dist
-Author: Trading Economics
-Author-email: support@tradingeconomics.com
-License: MIT
-Keywords: tradingeconomics,data
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-=====================
-Trading Economics API
-=====================
-
-The Trading Economics Python package provides direct access to over 300,000 economic indicators, exchange rates, stock market indexes, government bond yields, and commodity prices. This package offers various request methods to query the Trading Economics databases and supports exporting data in XML, CSV, or JSON format. The API can be used to feed custom-developed applications, public websites, or off-the-shelf software.
-
-
-Installation
-----------------------------------------
-
-You can install the package using pip:
-
-    - pip install tradingeconomics
-
-
-Authentication
-----------------------------------------
-
-To use the Trading Economics API, you need to authenticate by providing your API key and secret:
-
-    - import tradingeconomics as te
-    - te.login('key:secret')
-
-
-Sample Usage
-----------------------------------------
-
-Here are some examples of how to use the Trading Economics Python package:
-
-    - te.getCalendarData()
-    - te.getIndicatorData(country=['mexico', 'sweden'], output_type='df')
-    - te.getMarketsData(marketsField='commodities')
-    - te.getMarketsBySymbol(symbols='aapl:us')
-    - te.getFinancialsData(symbol='aapl:us', output_type='df')
-
-
-GitHub Examples
-----------------------------------------
-
-You can find additional examples and usage instructions in the GitHub repository:
- - https://github.com/tradingeconomics/tradingeconomics-python/tree/main/examples
-
-
-Documentation
-----------------------------------------
-
-For detailed documentation and API reference, please visit the Trading Economics API documentation:
- - https://docs.tradingeconomics.com
+Metadata-Version: 2.1
+Name: tradingeconomics
+Version: 4.2.9
+Summary: Trading Economics API
+Home-page: https://github.com/tradingeconomics/tradingeconomics-python
+Download-URL: https://github.com/tradingeconomics/tradingeconomics-python/tree/main/dist
+Author: Trading Economics
+Author-email: support@tradingeconomics.com
+License: MIT
+Keywords: tradingeconomics,data
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.2
+Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+=====================
+Trading Economics API
+=====================
+
+The Trading Economics Python package provides direct access to over 300,000 economic indicators, exchange rates, stock market indexes, government bond yields, and commodity prices. This package offers various request methods to query the Trading Economics databases and supports exporting data in XML, CSV, or JSON format. The API can be used to feed custom-developed applications, public websites, or off-the-shelf software.
+
+
+Installation
+----------------------------------------
+
+You can install the package using pip:
+
+    - pip install tradingeconomics
+
+
+Authentication
+----------------------------------------
+
+To use the Trading Economics API, you need to authenticate by providing your API key and secret:
+
+    - import tradingeconomics as te
+    - te.login('key:secret')
+
+
+Sample Usage
+----------------------------------------
+
+Here are some examples of how to use the Trading Economics Python package:
+
+    - te.getCalendarData()
+    - te.getIndicatorData(country=['mexico', 'sweden'], output_type='df')
+    - te.getMarketsData(marketsField='commodities')
+    - te.getMarketsBySymbol(symbols='aapl:us')
+    - te.getFinancialsData(symbol='aapl:us', output_type='df')
+
+
+GitHub Examples
+----------------------------------------
+
+You can find additional examples and usage instructions in the GitHub repository:
+ - https://github.com/tradingeconomics/tradingeconomics-python/tree/main/examples
+
+
+Documentation
+----------------------------------------
+
+For detailed documentation and API reference, please visit the Trading Economics API documentation:
+ - https://docs.tradingeconomics.com
```

### Comparing `tradingeconomics-4.2.8/README.rst` & `tradingeconomics-4.2.9/README.rst`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-=====================
-Trading Economics API
-=====================
-
-The Trading Economics Python package provides direct access to over 300,000 economic indicators, exchange rates, stock market indexes, government bond yields, and commodity prices. This package offers various request methods to query the Trading Economics databases and supports exporting data in XML, CSV, or JSON format. The API can be used to feed custom-developed applications, public websites, or off-the-shelf software.
-
-
-Installation
-----------------------------------------
-
-You can install the package using pip:
-
-    - pip install tradingeconomics
-
-
-Authentication
-----------------------------------------
-
-To use the Trading Economics API, you need to authenticate by providing your API key and secret:
-
-    - import tradingeconomics as te
-    - te.login('key:secret')
-
-
-Sample Usage
-----------------------------------------
-
-Here are some examples of how to use the Trading Economics Python package:
-
-    - te.getCalendarData()
-    - te.getIndicatorData(country=['mexico', 'sweden'], output_type='df')
-    - te.getMarketsData(marketsField='commodities')
-    - te.getMarketsBySymbol(symbols='aapl:us')
-    - te.getFinancialsData(symbol='aapl:us', output_type='df')
-
-
-GitHub Examples
-----------------------------------------
-
-You can find additional examples and usage instructions in the GitHub repository:
- - https://github.com/tradingeconomics/tradingeconomics-python/tree/main/examples
-
-
-Documentation
-----------------------------------------
-
-For detailed documentation and API reference, please visit the Trading Economics API documentation:
+=====================
+Trading Economics API
+=====================
+
+The Trading Economics Python package provides direct access to over 300,000 economic indicators, exchange rates, stock market indexes, government bond yields, and commodity prices. This package offers various request methods to query the Trading Economics databases and supports exporting data in XML, CSV, or JSON format. The API can be used to feed custom-developed applications, public websites, or off-the-shelf software.
+
+
+Installation
+----------------------------------------
+
+You can install the package using pip:
+
+    - pip install tradingeconomics
+
+
+Authentication
+----------------------------------------
+
+To use the Trading Economics API, you need to authenticate by providing your API key and secret:
+
+    - import tradingeconomics as te
+    - te.login('key:secret')
+
+
+Sample Usage
+----------------------------------------
+
+Here are some examples of how to use the Trading Economics Python package:
+
+    - te.getCalendarData()
+    - te.getIndicatorData(country=['mexico', 'sweden'], output_type='df')
+    - te.getMarketsData(marketsField='commodities')
+    - te.getMarketsBySymbol(symbols='aapl:us')
+    - te.getFinancialsData(symbol='aapl:us', output_type='df')
+
+
+GitHub Examples
+----------------------------------------
+
+You can find additional examples and usage instructions in the GitHub repository:
+ - https://github.com/tradingeconomics/tradingeconomics-python/tree/main/examples
+
+
+Documentation
+----------------------------------------
+
+For detailed documentation and API reference, please visit the Trading Economics API documentation:
  - https://docs.tradingeconomics.com
```

### Comparing `tradingeconomics-4.2.8/setup.py` & `tradingeconomics-4.2.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from setuptools import setup, find_packages
-from os import path
-import io
-
-def readme():
-    this_directory = path.abspath(path.dirname(__file__))
-    with io.open(path.join(this_directory, 'README.rst'), encoding='utf-8') as f:
-      return f.read()
-
-setup(
-  name = 'tradingeconomics',
-  packages = find_packages(exclude=['tests*']),  
-  version = '4.2.8',
-  description = 'Trading Economics API',
-  long_description =readme(),
-  long_description_content_type='text/x-rst',
-  author = 'Trading Economics',
-  author_email = 'support@tradingeconomics.com',
-  license = 'MIT',
-  url = 'https://github.com/tradingeconomics/tradingeconomics-python', 
-  download_url = 'https://github.com/tradingeconomics/tradingeconomics-python/tree/main/dist',
-  keywords = ['tradingeconomics', 'data'], 
-  classifiers = [ 'Programming Language :: Python :: 3',
-                'Programming Language :: Python :: 3.2',
-                'Programming Language :: Python :: 3.3',
-                'Programming Language :: Python :: 3.4',
-                'Programming Language :: Python :: 3.8'],
-  install_requires = ['pandas', 'websocket-client'],
-)
+from setuptools import setup, find_packages
+from os import path
+import io
+
+def readme():
+    this_directory = path.abspath(path.dirname(__file__))
+    with io.open(path.join(this_directory, 'README.rst'), encoding='utf-8') as f:
+      return f.read()
+
+setup(
+  name = 'tradingeconomics',
+  packages = find_packages(exclude=['tests*']),  
+  version = '4.2.9',
+  description = 'Trading Economics API',
+  long_description =readme(),
+  long_description_content_type='text/x-rst',
+  author = 'Trading Economics',
+  author_email = 'support@tradingeconomics.com',
+  license = 'MIT',
+  url = 'https://github.com/tradingeconomics/tradingeconomics-python', 
+  download_url = 'https://github.com/tradingeconomics/tradingeconomics-python/tree/main/dist',
+  keywords = ['tradingeconomics', 'data'], 
+  classifiers = [ 'Programming Language :: Python :: 3',
+                'Programming Language :: Python :: 3.2',
+                'Programming Language :: Python :: 3.3',
+                'Programming Language :: Python :: 3.4',
+                'Programming Language :: Python :: 3.8'],
+  install_requires = ['pandas', 'websocket-client'],
+)
```

### Comparing `tradingeconomics-4.2.8/tradingeconomics/__init__.py` & `tradingeconomics-4.2.9/tradingeconomics/__init__.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-"""
-This package allows Trading Economics clients to easily query the Trading Economics API to get data into their Python code.
-"""
-
-import sys
-
-PY3 = sys.version_info[0] == 3
-
-
-if PY3: # Python 3+
-    from .historicalDB import getHistorical
-    from .historical import getHistoricalData, getHistoricalRatings,getHistoricalByTicker,getHistoricalUpdates
-    from .calendar import getCalendarData, getCalendarId,getCalendarUpdates, getCalendarEventsByGroup
-    from .forecasts import getForecastData,getForecastByTicker
-    from .indicators import getIndicatorData, getRatings, getLatestUpdates, getDiscontinuedIndicator, getIndicatorByCategoryGroup, getIndicatorByTicker, getPeers, getAllCountries
-    from .markets import getMarketsData, getMarketsBySymbol, getMarketsIntraday, getMarketsPeers, getMarketsComponents, getMarketsSearch, getMarketsForecasts, getCurrencyCross, getMarketsIntradayByInterval, getMarketsStockDescriptions,getMarketsSymbology,getStocksByCountry
-    from .historicalMarkets import fetchMarkets
-    from .glob import login, subscribe
-    from .stream import run
-    from .earnings import getEarnings, getEarningsType
-    from .news import getNews, getArticles, getArticleId 
-    from .worldBank import getWBCategories, getWBIndicator, getWBCountry, getWBHistorical
-    from .comtrade import getCmtCategories, getCmtCountry, getCmtHistorical, getCmtTwoCountries, getCmtUpdates, getCmtCountryByCategory, getCmtTotalByType, getCmtCountryFilterByType, getCmtSnapshotByType
-    from .federalReserve import getFedRStates, getFedRSnaps, getFedRHistorical, getFedRCounty
-    from .eurostat import getEurostatData,getEurostatCountries,getEurostatCategoryGroups
-    from .historicalEurostat import getHistoricalEurostat
-    from .financials import getFinancialsData, getFinancialsCategoryList, getFinancialsDataByCategory, getSectors
-    from .historicalFinancials import getFinancialsHistorical
-    from .search import getSearch
-
-
-else: # Python 2.X
-    from historicalDB import getHistorical
-    from historical import getHistoricalData, getHistoricalRatings,getHistoricalByTicker
-    from calendar import getCalendarData, getCalendarId, getCalendarUpdates
-    from forecasts import getForecastData,getForecastByTicker
-    from indicators import getIndicatorData, getRatings, getLatestUpdates, getDiscontinuedIndicator, getIndicatorByCategoryGroup,getIndicatorByTicker, getPeers
-    from markets import getMarketsData, getMarketsBySymbol, getMarketsIntraday, getMarketsPeers, getMarketsComponents, getMarketsSearch, getMarketsForecasts, getCurrencyCross, getMarketsIntradayByInterval, getMarketsStockDescriptions
-    from historicalMarkets import fetchMarkets
-    from glob import login, subscribe
-    from stream import run
-    from earnings import getEarnings, getEarningsType
-    from news import getNews, getArticles, getArticleId
-    from worldBank import getWBCategories, getWBIndicator, getWBCountry, getWBHistorical
-    from comtrade import getCmtCategories, getCmtCountry, getCmtHistorical, getCmtTwoCountries, getCmtUpdates, getCmtCountryByCategory, getCmtTotalByType, getCmtCountryFilterByType, getCmtSnapshotByType
-    from federalReserve import getFedRStates, getFedRSnaps, getFedRHistorical, getFedRCounty
-    from eurostat import getEurostatData,getEurostatCountries,getEurostatCategoryGroups
-    from historicalEurostat import getHistoricalEurostat
-    from financials import getFinancialsData, getFinancialsCategoryList, getFinancialsDataByCategory
-    from historicalFinancials import getFinancialsHistorical
-    from search import getSearch
-
-
-
-
+"""
+This package allows Trading Economics clients to easily query the Trading Economics API to get data into their Python code.
+"""
+
+import sys
+
+PY3 = sys.version_info[0] == 3
+
+
+if PY3: # Python 3+
+    from .historicalDB import getHistorical
+    from .historical import getHistoricalData, getHistoricalRatings,getHistoricalByTicker,getHistoricalUpdates
+    from .calendar import getCalendarData, getCalendarId,getCalendarUpdates, getCalendarEventsByGroup
+    from .forecasts import getForecastData,getForecastByTicker
+    from .indicators import getIndicatorData, getRatings, getLatestUpdates, getDiscontinuedIndicator, getIndicatorByCategoryGroup, getIndicatorByTicker, getPeers, getAllCountries
+    from .markets import getMarketsData, getMarketsBySymbol, getMarketsIntraday, getMarketsPeers, getMarketsComponents, getMarketsSearch, getMarketsForecasts, getCurrencyCross, getMarketsIntradayByInterval, getMarketsStockDescriptions,getMarketsSymbology,getStocksByCountry
+    from .historicalMarkets import fetchMarkets
+    from .glob import login, subscribe
+    from .stream import run
+    from .earnings import getEarnings, getEarningsType
+    from .news import getNews, getArticles, getArticleId 
+    from .worldBank import getWBCategories, getWBIndicator, getWBCountry, getWBHistorical
+    from .comtrade import getCmtCategories, getCmtCountry, getCmtHistorical, getCmtTwoCountries, getCmtUpdates, getCmtCountryByCategory, getCmtTotalByType, getCmtCountryFilterByType, getCmtSnapshotByType
+    from .federalReserve import getFedRStates, getFedRSnaps, getFedRHistorical, getFedRCounty
+    from .eurostat import getEurostatData,getEurostatCountries,getEurostatCategoryGroups
+    from .historicalEurostat import getHistoricalEurostat
+    from .financials import getFinancialsData, getFinancialsCategoryList, getFinancialsDataByCategory, getSectors
+    from .historicalFinancials import getFinancialsHistorical
+    from .search import getSearch
+
+
+else: # Python 2.X
+    from historicalDB import getHistorical
+    from historical import getHistoricalData, getHistoricalRatings,getHistoricalByTicker
+    from calendar import getCalendarData, getCalendarId, getCalendarUpdates
+    from forecasts import getForecastData,getForecastByTicker
+    from indicators import getIndicatorData, getRatings, getLatestUpdates, getDiscontinuedIndicator, getIndicatorByCategoryGroup,getIndicatorByTicker, getPeers
+    from markets import getMarketsData, getMarketsBySymbol, getMarketsIntraday, getMarketsPeers, getMarketsComponents, getMarketsSearch, getMarketsForecasts, getCurrencyCross, getMarketsIntradayByInterval, getMarketsStockDescriptions
+    from historicalMarkets import fetchMarkets
+    from glob import login, subscribe
+    from stream import run
+    from earnings import getEarnings, getEarningsType
+    from news import getNews, getArticles, getArticleId
+    from worldBank import getWBCategories, getWBIndicator, getWBCountry, getWBHistorical
+    from comtrade import getCmtCategories, getCmtCountry, getCmtHistorical, getCmtTwoCountries, getCmtUpdates, getCmtCountryByCategory, getCmtTotalByType, getCmtCountryFilterByType, getCmtSnapshotByType
+    from federalReserve import getFedRStates, getFedRSnaps, getFedRHistorical, getFedRCounty
+    from eurostat import getEurostatData,getEurostatCountries,getEurostatCategoryGroups
+    from historicalEurostat import getHistoricalEurostat
+    from financials import getFinancialsData, getFinancialsCategoryList, getFinancialsDataByCategory
+    from historicalFinancials import getFinancialsHistorical
+    from search import getSearch
+
+
+
+
```

### Comparing `tradingeconomics-4.2.8/tradingeconomics/calendar.py` & `tradingeconomics-4.2.9/tradingeconomics/calendar.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,308 +1,308 @@
-import sys
-from datetime import *
-from . import functions as fn
-from . import glob
-import ssl
-
-
-PY3 = sys.version_info[0] == 3
-
-if PY3: # Python 3+
-    from urllib.parse import quote
-else: # Python 2.X
-    from urllib import quote
-
-
-class ParametersError(ValueError):
-    pass
-
-class DateError(ValueError):
-    pass
-
-class CredentialsError(ValueError):
-    pass
-
-class LoginError(AttributeError):
-    pass
-
-class WebRequestError(ValueError):
-    pass
-
-
-
-def paramCheck (country, indicator = None):
-    if type(country) is str and indicator == None:
-        linkAPI = 'https://api.tradingeconomics.com/calendar/country/' + quote(country)
-    elif type(country) is not str and indicator == None:
-        multiCountry = ",".join(country)
-        linkAPI = 'https://api.tradingeconomics.com/calendar/country/' + quote(multiCountry)
-    elif type(country) is not str and type(indicator) is str:  
-        multiCountry = ",".join(country)
-        linkAPI = 'https://api.tradingeconomics.com/calendar/country/' + quote(multiCountry) + '/indicator/' + quote(indicator)
-    elif type(country) is str and type(indicator) is not str:
-        multiIndicator = ",".join(indicator)
-        linkAPI = 'https://api.tradingeconomics.com/calendar/country/' + quote(country) + '/indicator/' + quote(multiIndicator) 
-    else:
-        multiCountry = ",".join(country)
-        multiIndicator = ",".join(indicator)
-        linkAPI = 'https://api.tradingeconomics.com/calendar/country/' + quote(multiCountry) + '/indicator/' + quote(multiIndicator)
-    return linkAPI
-        
-def checkCalendarId(id):
-    linkAPI = 'https://api.tradingeconomics.com/calendar/calendarid'      
-    if type(id) is str:
-        linkAPI +=  '/' + quote(str(id))
-    else:
-        linkAPI += '/' + quote(",".join(id))
-    return linkAPI
-
-def getCalendarId(id = None, output_type = None):
-    
-    """
-    Return calendar events by it's specific Id.
-    ===========================================================
-
-    Parameters:
-    -----------
-    Id: Specific Id or Ids.
-    output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries without any parsing. 
-
-    Notes
-    -----
-    All parameters are optional. When not supplying parameters, data for all calendar events will be provided. 
-
-    Example
-    -------
-    getCalendarId(id = None, output_type = None)
-
-    getCalendarId(id = 160025, output_type = None)
-
-    getCalendarId(id = ['174108','160025','160030'], output_type = 'df')
-    
-    """
-    
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-
-    if id == None:
-        linkAPI = 'https://api.tradingeconomics.com/calendar'
-    else:
-        linkAPI = checkCalendarId(id)
-   
-    try:
-        linkAPI += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-    
-    try:
-        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
-    except Exception as e:
-        print(e)
-        
-
-def getCalendarData(country = None, category = None, initDate = None, endDate = None, importance=None, ticker=None, output_type = None, values=None):
-    """
-    Returns Lastest Updates by country, by country and initial date, by initial date only.
-    =================================================================================
-    Parameters:
-    -----------
-        country: string or list.
-                country = 'united states'
-                country = ['united states', 'portugal']
-        category: string
-                category='inflation rate'
-        ticker: string or list.
-                ticker = 'IJCUSA'
-                ticker=['IJCUSA','SPAINFACORD','BAHRAININFNRATE']
-        importance: string.
-                importance = '2'
-        values: boolean.
-                values = True
-                values = False
-        
-        initDate: string.
-                initDate = '2021-01-01'
-        endDate:string.
-                endDate = '2021-01-03'
-        
-        output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web. 
-    Notes
-    -----
-    all parameters are optional.
-    
-    Example
-    -------
-            getCalendarData(output_type='df')
-            getCalendarData(importance='2', output_type='df')
-            getCalendarData(country='all', initDate = '2011-01-01', endDate = '2016-01-01', output_type='df')
-            getCalendarData(initDate='2016-01-01', endDate='2016-01-01',importance='3', output_type='df')
-            getCalendarData(country='united states',  output_type='df')
-            getCalendarData(country = 'United States', initDate = '2011-01-01', endDate = '2016-01-01', output_type='df')
-            getCalendarData(country='united states',initDate='2016-01-01', endDate='2016-01-01',importance='3', output_type='df')
-            getCalendarData(category='inflation rate', output_type='df')
-            getCalendarData(category='inflation rate',importance='2', output_type='df')
-            getCalendarData(category='inflation rate',initDate='2016-03-01', endDate='2016-03-03', output_type='df')
-            getCalendarData(category='inflation rate',initDate='2016-03-01', endDate='2016-03-03',importance='2', output_type='df')
-            getCalendarData(country = ['United States','china'], output_type='df')
-            getCalendarData(country=['united states','china'], importance='2', output_type='df')
-            getCalendarData(country=['united states', 'china'], initDate = '2016-01-01', endDate = '2016-01-03', output_type='df')
-            getCalendarData(country=['united states', 'china'], initDate = '2016-01-01', endDate = '2016-01-03',importance=2, output_type='df')
-            getCalendarData(country = 'United States', category = 'initial jobless claims', output_type='df')
-            getCalendarData(country = 'United States', category = 'initial jobless claims',initDate = '2011-01-01', endDate = '2016-01-01', output_type='df')
-            getCalendarData(ticker=['IJCUSA','SPAINFACORD','BAHRAININFNRATE'], output_type='df')
-            getCalendarData(ticker=['IJCUSA','SPAINFACORD','BAHRAININFNRATE'], initDate = '2021-01-01', endDate = '2021-01-03',utput_type='df')
-    """
-            
-    
-    # d is a dictionary used for create the api url
-    d = {
-        'url_base': 'https://api.tradingeconomics.com/calendar',
-        'country': '',
-        'category' : '',
-        'init_date': '',
-        'end_date':'',
-        'importance':'',
-        'ticker':'',
-        'key': f'?c={glob.apikey}',
-        'output_type' : '',
-        'values': ''
-    }
-    if initDate and endDate :     
-
-        fn.validate(initDate)
-        fn.validate(endDate)
-        fn.validatePeriod(initDate, endDate)
-        d['init_date']=f'/{initDate}'
-        d['end_date']=f'/{endDate}'
-
-    if ticker:
-        d['ticker'] = f'/ticker/{fn.stringOrList(ticker)}'
-        api_url_request = "%s%s%s%s%s" % (d['url_base'],  d['ticker'],  d['init_date'],  d['end_date'],  d['key']) 
-        #print(api_url_request)
-        return fn.dataRequest(api_request=api_url_request, output_type=output_type)
-
-    if country:
-        d['country']=f'/country/{fn.stringOrList(country)}'
-        
-    if category:
-        d['category'] = f'/indicator/{fn.stringOrList(category)}'
-    if importance:
-        d['importance'] = f'&importance={importance}'
-
-    if initDate and endDate and not country and not category:
-        d['country'] = f'/country/all'
-
-    if values:
-        d['values'] = f'&values=true'
-    elif values == False:
-        d['values'] = f'&values=false'
-
-    api_url_request = "%s%s%s%s%s%s%s%s" % (d['url_base'], d['country'], d['category'],  d['init_date'],  d['end_date'],  d['key'], d['importance'], d['values']) 
-    return fn.dataRequest(api_request=api_url_request, output_type=output_type)
-
-
-def getCalendarUpdates(output_type = None):
-    """
-    Returns Lastest Calendar Updates
-    =================================================================================
-    Parameters:
-    -----------
-        
-        
-        output_type: string.
-             'dict'(default) for dictionary format output, 
-             'df' for data frame,
-             'raw' for list of dictionaries directly from the web. 
-    Notes
-    -----
-    
-    
-    Example
-    -------
-            getCalendarData(output_type='df')
-            
-    """
-            
-    
-    # d is a dictionary used for create the api url
-    d = {
-        'url_base': 'https://api.tradingeconomics.com/calendar/updates',
-        'key': f'?c={glob.apikey}',
-        'output_type' : ''
-    }
-
-    api_url_request = "%s%s" % (d['url_base'], d['key']) 
-
-    return fn.dataRequest(api_request=api_url_request, output_type=output_type)
-    #return
-
-
-
-def getCalendarEventsByGroup(group: str, country: str=None, initDate = None, endDate = None, output_type = None):
-    """
-    Returns calendar events of the specified group
-    =================================================================================
-    Parameters:
-    -----------
-        group: string
-            bonds, inflation
-
-        country: string, optional
-            'united states'
-            'china'
-        
-        
-        output_type: string.
-             'dict'(default) for dictionary format output, 
-             'df' for data frame,
-             'raw' for list of dictionaries directly from the web. 
-    Notes
-    -----
-    
-    
-    Example
-    -------
-            getCalendarEventsByGroup(output_type='df')
-            getCalendarEventsByGroup(country='china', group='inflation', endDate='2023-02-01', output_type='df')
-            getCalendarEventsByGroup('inflation', initDate='2023-01-01', endDate='2023-02-01', output_type='dict')
-            
-    """
-
-    d = {
-            'url_base': 'https://api.tradingeconomics.com/calendar',
-            'key': f'?c={glob.apikey}',
-            'output_type' : ''
-        }
-
-    api_url_request = f"{d['url_base']}"
-
-    if country:
-        api_url_request += f"/country/{fn.stringOrList(country)}"
-    
-    if group:
-        api_url_request += f'/group/{fn.stringOrList(group)}'
-    else:
-        return 'Group cannot be empty'
-
-    if initDate and endDate:
-        fn.validatePeriod(initDate, endDate)
-    
-    if initDate:
-        fn.validate(initDate)
-        api_url_request += f"/{initDate}"
-    
-    if endDate:
-        fn.validate(endDate)
-        api_url_request += f'/{endDate}'
-    
-    api_url_request += f"{d['key']}"
-    
+import sys
+from datetime import *
+from . import functions as fn
+from . import glob
+import ssl
+
+
+PY3 = sys.version_info[0] == 3
+
+if PY3: # Python 3+
+    from urllib.parse import quote
+else: # Python 2.X
+    from urllib import quote
+
+
+class ParametersError(ValueError):
+    pass
+
+class DateError(ValueError):
+    pass
+
+class CredentialsError(ValueError):
+    pass
+
+class LoginError(AttributeError):
+    pass
+
+class WebRequestError(ValueError):
+    pass
+
+
+
+def paramCheck (country, indicator = None):
+    if type(country) is str and indicator == None:
+        linkAPI = 'https://api.tradingeconomics.com/calendar/country/' + quote(country)
+    elif type(country) is not str and indicator == None:
+        multiCountry = ",".join(country)
+        linkAPI = 'https://api.tradingeconomics.com/calendar/country/' + quote(multiCountry)
+    elif type(country) is not str and type(indicator) is str:  
+        multiCountry = ",".join(country)
+        linkAPI = 'https://api.tradingeconomics.com/calendar/country/' + quote(multiCountry) + '/indicator/' + quote(indicator)
+    elif type(country) is str and type(indicator) is not str:
+        multiIndicator = ",".join(indicator)
+        linkAPI = 'https://api.tradingeconomics.com/calendar/country/' + quote(country) + '/indicator/' + quote(multiIndicator) 
+    else:
+        multiCountry = ",".join(country)
+        multiIndicator = ",".join(indicator)
+        linkAPI = 'https://api.tradingeconomics.com/calendar/country/' + quote(multiCountry) + '/indicator/' + quote(multiIndicator)
+    return linkAPI
+        
+def checkCalendarId(id):
+    linkAPI = 'https://api.tradingeconomics.com/calendar/calendarid'      
+    if type(id) is str:
+        linkAPI +=  '/' + quote(str(id))
+    else:
+        linkAPI += '/' + quote(",".join(id))
+    return linkAPI
+
+def getCalendarId(id = None, output_type = None):
+    
+    """
+    Return calendar events by it's specific Id.
+    ===========================================================
+
+    Parameters:
+    -----------
+    Id: Specific Id or Ids.
+    output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries without any parsing. 
+
+    Notes
+    -----
+    All parameters are optional. When not supplying parameters, data for all calendar events will be provided. 
+
+    Example
+    -------
+    getCalendarId(id = None, output_type = None)
+
+    getCalendarId(id = 160025, output_type = None)
+
+    getCalendarId(id = ['174108','160025','160030'], output_type = 'df')
+    
+    """
+    
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+
+    if id == None:
+        linkAPI = 'https://api.tradingeconomics.com/calendar'
+    else:
+        linkAPI = checkCalendarId(id)
+   
+    try:
+        linkAPI += '?c=' + glob.apikey
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+    
+    try:
+        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
+    except Exception as e:
+        print(e)
+        
+
+def getCalendarData(country = None, category = None, initDate = None, endDate = None, importance=None, ticker=None, output_type = None, values=None):
+    """
+    Returns Lastest Updates by country, by country and initial date, by initial date only.
+    =================================================================================
+    Parameters:
+    -----------
+        country: string or list.
+                country = 'united states'
+                country = ['united states', 'portugal']
+        category: string
+                category='inflation rate'
+        ticker: string or list.
+                ticker = 'IJCUSA'
+                ticker=['IJCUSA','SPAINFACORD','BAHRAININFNRATE']
+        importance: string.
+                importance = '2'
+        values: boolean.
+                values = True
+                values = False
+        
+        initDate: string.
+                initDate = '2021-01-01'
+        endDate:string.
+                endDate = '2021-01-03'
+        
+        output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+    Notes
+    -----
+    all parameters are optional.
+    
+    Example
+    -------
+            getCalendarData(output_type='df')
+            getCalendarData(importance='2', output_type='df')
+            getCalendarData(country='all', initDate = '2011-01-01', endDate = '2016-01-01', output_type='df')
+            getCalendarData(initDate='2016-01-01', endDate='2016-01-01',importance='3', output_type='df')
+            getCalendarData(country='united states',  output_type='df')
+            getCalendarData(country = 'United States', initDate = '2011-01-01', endDate = '2016-01-01', output_type='df')
+            getCalendarData(country='united states',initDate='2016-01-01', endDate='2016-01-01',importance='3', output_type='df')
+            getCalendarData(category='inflation rate', output_type='df')
+            getCalendarData(category='inflation rate',importance='2', output_type='df')
+            getCalendarData(category='inflation rate',initDate='2016-03-01', endDate='2016-03-03', output_type='df')
+            getCalendarData(category='inflation rate',initDate='2016-03-01', endDate='2016-03-03',importance='2', output_type='df')
+            getCalendarData(country = ['United States','china'], output_type='df')
+            getCalendarData(country=['united states','china'], importance='2', output_type='df')
+            getCalendarData(country=['united states', 'china'], initDate = '2016-01-01', endDate = '2016-01-03', output_type='df')
+            getCalendarData(country=['united states', 'china'], initDate = '2016-01-01', endDate = '2016-01-03',importance=2, output_type='df')
+            getCalendarData(country = 'United States', category = 'initial jobless claims', output_type='df')
+            getCalendarData(country = 'United States', category = 'initial jobless claims',initDate = '2011-01-01', endDate = '2016-01-01', output_type='df')
+            getCalendarData(ticker=['IJCUSA','SPAINFACORD','BAHRAININFNRATE'], output_type='df')
+            getCalendarData(ticker=['IJCUSA','SPAINFACORD','BAHRAININFNRATE'], initDate = '2021-01-01', endDate = '2021-01-03',utput_type='df')
+    """
+            
+    
+    # d is a dictionary used for create the api url
+    d = {
+        'url_base': 'https://api.tradingeconomics.com/calendar',
+        'country': '',
+        'category' : '',
+        'init_date': '',
+        'end_date':'',
+        'importance':'',
+        'ticker':'',
+        'key': f'?c={glob.apikey}',
+        'output_type' : '',
+        'values': ''
+    }
+    if initDate and endDate :     
+
+        fn.validate(initDate)
+        fn.validate(endDate)
+        fn.validatePeriod(initDate, endDate)
+        d['init_date']=f'/{initDate}'
+        d['end_date']=f'/{endDate}'
+
+    if ticker:
+        d['ticker'] = f'/ticker/{fn.stringOrList(ticker)}'
+        api_url_request = "%s%s%s%s%s" % (d['url_base'],  d['ticker'],  d['init_date'],  d['end_date'],  d['key']) 
+        #print(api_url_request)
+        return fn.dataRequest(api_request=api_url_request, output_type=output_type)
+
+    if country:
+        d['country']=f'/country/{fn.stringOrList(country)}'
+        
+    if category:
+        d['category'] = f'/indicator/{fn.stringOrList(category)}'
+    if importance:
+        d['importance'] = f'&importance={importance}'
+
+    if initDate and endDate and not country and not category:
+        d['country'] = f'/country/all'
+
+    if values:
+        d['values'] = f'&values=true'
+    elif values == False:
+        d['values'] = f'&values=false'
+
+    api_url_request = "%s%s%s%s%s%s%s%s" % (d['url_base'], d['country'], d['category'],  d['init_date'],  d['end_date'],  d['key'], d['importance'], d['values']) 
+    return fn.dataRequest(api_request=api_url_request, output_type=output_type)
+
+
+def getCalendarUpdates(output_type = None):
+    """
+    Returns Lastest Calendar Updates
+    =================================================================================
+    Parameters:
+    -----------
+        
+        
+        output_type: string.
+             'dict'(default) for dictionary format output, 
+             'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+    Notes
+    -----
+    
+    
+    Example
+    -------
+            getCalendarData(output_type='df')
+            
+    """
+            
+    
+    # d is a dictionary used for create the api url
+    d = {
+        'url_base': 'https://api.tradingeconomics.com/calendar/updates',
+        'key': f'?c={glob.apikey}',
+        'output_type' : ''
+    }
+
+    api_url_request = "%s%s" % (d['url_base'], d['key']) 
+
+    return fn.dataRequest(api_request=api_url_request, output_type=output_type)
+    #return
+
+
+
+def getCalendarEventsByGroup(group: str, country: str=None, initDate = None, endDate = None, output_type = None):
+    """
+    Returns calendar events of the specified group
+    =================================================================================
+    Parameters:
+    -----------
+        group: string
+            bonds, inflation
+
+        country: string, optional
+            'united states'
+            'china'
+        
+        
+        output_type: string.
+             'dict'(default) for dictionary format output, 
+             'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+    Notes
+    -----
+    
+    
+    Example
+    -------
+            getCalendarEventsByGroup(output_type='df')
+            getCalendarEventsByGroup(country='china', group='inflation', endDate='2023-02-01', output_type='df')
+            getCalendarEventsByGroup('inflation', initDate='2023-01-01', endDate='2023-02-01', output_type='dict')
+            
+    """
+
+    d = {
+            'url_base': 'https://api.tradingeconomics.com/calendar',
+            'key': f'?c={glob.apikey}',
+            'output_type' : ''
+        }
+
+    api_url_request = f"{d['url_base']}"
+
+    if country:
+        api_url_request += f"/country/{fn.stringOrList(country)}"
+    
+    if group:
+        api_url_request += f'/group/{fn.stringOrList(group)}'
+    else:
+        return 'Group cannot be empty'
+
+    if initDate and endDate:
+        fn.validatePeriod(initDate, endDate)
+    
+    if initDate:
+        fn.validate(initDate)
+        api_url_request += f"/{initDate}"
+    
+    if endDate:
+        fn.validate(endDate)
+        api_url_request += f'/{endDate}'
+    
+    api_url_request += f"{d['key']}"
+    
     return fn.dataRequest(api_request=api_url_request, output_type=output_type)
```

### Comparing `tradingeconomics-4.2.8/tradingeconomics/comtrade.py` & `tradingeconomics-4.2.9/tradingeconomics/indicators.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,545 +1,464 @@
-import json
-import urllib
-import pandas as pd
-import sys
-from datetime import *
-from . import functions as fn
-from . import glob
-import ssl
-
-PY3 = sys.version_info[0] == 3
-
-if PY3:  # Python 3+
-    from urllib.request import urlopen
-    from urllib.parse import quote
-else:  # Python 2.X
-    from urllib import urlopen
-    from urllib import quote
-
-
-class ParametersError(ValueError):
-    pass
-
-
-class CredentialsError(ValueError):
-    pass
-
-
-class LoginError(AttributeError):
-    pass
-
-class TypeError(AttributeError):
-    pass
-
-
-class WebRequestError(ValueError):
-    pass
-
-
-def checkCmtCountry(country):
-    linkAPI = 'https://api.tradingeconomics.com/comtrade/country/'
-
-    if type(country) is str:
-        linkAPI += quote(country)
-    else:
-        linkAPI += quote("/".join(country), safe='')
-    return linkAPI
-
-
-def checkCmtPage(linkAPI, page_number):
-    if page_number != None:
-        linkAPI += '/{0}'.format(page_number)
-
-    return linkAPI
-
-
-def getCmtUpdates(output_type=None):
-    """
-    Get latest updates information on Comtrade.
-    =================================================================================
-
-    Parameters:
-    -----------
-    output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web.
-
-    Notes
-    -----
-    with no parameters a list of last updates will be given.
-
-    Example
-    -------
-    getCmtUpdates(output_type = None)
-
-    """
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-
-    linkAPI = 'https://api.tradingeconomics.com/comtrade/updates'
-    try:
-        linkAPI += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-
-    try:
-        # print(linkAPI)
-        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
-    except Exception as e:
-        print(e)
-        
-
-
-
-def getCmtCategories(category=None, output_type=None):
-    """
-    Get detailed information about Comtrade categories.
-    =================================================================================
-
-    Parameters:
-    -----------
-    category:list.
-                List of strings of all categories.
-    output_type: string.
-                'dict'(default) for dictionary format output, 'df' for data frame,
-                'raw' for list of dictionaries directly from the web.
-
-    Notes
-    -----
-    A list of all categories will be given.
-
-    Example
-    -------
-    getCmtCategories(category = None, output_type = None)
-
-    """
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-
-    linkAPI = 'https://api.tradingeconomics.com/comtrade/categories'
-
-    if category == None:
-        linkAPI = 'https://api.tradingeconomics.com/comtrade/categories/'
-
-    try:
-        linkAPI += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-
-    try:
-        # print(linkAPI)
-        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
-    except Exception as e:
-        print(e)
-
-
-def getCmtCountry(country=None, page_number=None, output_type=None):
-    """
-    Get detailed information about Comtrade countries.
-    =================================================================================
-
-    Parameters:
-    -----------
-    country:list.
-             List of strings of all categories or one country with pagination.
-             for example:
-                country = 'country_name' , page_number = 3
-                country = ['country_name', 'country_name'], page_number = 3
-    output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web.
-
-    Notes
-    -----
-    with no parameters a list of all categories will be given.
-
-    Example
-    -------
-    getCmtCountry(country = None, page_number = None, output_type = None)
-
-    getCmtCountry(country = 'china' , page_number = 3, output_type = None)
-
-    getCmtCountry(country = ['china', 'portugal'], page_number = 3, output_type = None)
-
-    """
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-
-    linkAPI = 'https://api.tradingeconomics.com/comtrade/countries'
-
-    if country == None:
-        linkAPI = 'https://api.tradingeconomics.com/comtrade/countries'
-    else:
-        linkAPI = checkCmtCountry(country)
-
-    if page_number != None:
-        linkAPI = checkCmtPage(linkAPI, page_number)
-    try:
-        linkAPI += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-
-    try:
-        #print(linkAPI)
-        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
-    except Exception as e:
-        print(e)
-
-
-def getCmtHistorical(symbol=None, output_type=None):
-    """
-    Get Historical data.
-    =================================================================================
-
-    Parameters:
-    -----------
-    symbol:list.
-             List of strings by a specific symbol.
-             for example:
-                symbol = 'te_symbol'
-    output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web.
-
-    Notes
-    -----
-    A symbol is required.
-
-    Example
-    -------
-    getCmtHistorical(symbol = 'PRTESP24031', output_type = None)
-
-    """
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-
-    linkAPI = 'https://api.tradingeconomics.com/comtrade/historical/'
-
-    if symbol == None:
-        return "A symbol is required!"
-    else:
-        linkAPI = 'https://api.tradingeconomics.com/comtrade/historical/' + quote(symbol)
-
-    try:
-        linkAPI += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-
-    try:
-        #print(linkAPI)
-        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
-    except Exception as e:
-        print(e)
-
-
-def getCmtTwoCountries(country1=None, country2=None, page_number=None, output_type=None):
-    """
-    Get detailed information about Comtrade between two countries.
-    =================================================================================
-
-    Parameters:
-    -----------
-    country:list.
-             List of strings of all categories between two countries with pagination.
-
-    output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web.
-
-    Example
-    -------
-    getCmtTwoCountries(country1 = 'portugal', country2 = 'spain', page_number = 3, output_type = None)
-
-    """
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-
-    linkAPI = 'https://api.tradingeconomics.com/comtrade/country'
-
-    if country1 and country2 == None:
-        linkAPI = 'https://api.tradingeconomics.com/comtrade/country'
-    else:
-        linkAPI = 'https://api.tradingeconomics.com/comtrade/country/' + quote(country1) + '/' + quote(country2)
-
-    if page_number != None:
-        linkAPI = checkCmtPage(linkAPI, page_number)
-
-    try:
-        linkAPI += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-
-    try:
-        #print(linkAPI)
-        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
-    except Exception as e:
-        print(e)
-
-
-def getCmtCountryByCategory(country=None, type=None, category=None, output_type=None):
-    """
-        Get detailed information about Comtrade Country by Imports or Exports and by Category
-        =================================================================================
-
-        Parameters:
-        -----------
-        country:string.
-                 for example:
-                    country = 'country_name'
-
-        type: string.
-                for example:
-                    type = 'import'
-                    type = 'export'
-        category: string.
-                for example:
-                    category = 'live animals'
-                    category = 'Swine, live'
-                    category = 'Sheep and goats, live'
-
-
-        output_type: string.
-                 'dict'(default) for dictionary format output, 'df' for data frame,
-                 'raw' for list of dictionaries directly from the web.
-
-        Notes
-        -----
-        'country' and 'type' parameters are not optional.
-        if 'category' is None, returns total exports or imports with main category
-
-        Example
-        -------
-        getCmtCountryByCategory(country = 'Portugal', type = 'import', category = None, output_type = None )
-
-        getCmtCountryByCategory(country = 'United States', type = 'export', category = 'live animals', output_type = 'raw')
-
-        getCmtCountryByCategory(country = 'Brazil', type = import, category = 'Swine, live', output_type = 'df' )
-
-        """
-
-    if country is None:
-        return f'country is missing'
-    if type is None:
-        return f"type is missing. Choose 'import' or 'export'"
-
-    def getLinkApi(country, type, category):
-        api_url_base = "https://api.tradingeconomics.com/comtrade"
-
-        if category is None:
-            return f'{api_url_base}/{type}/{quote(country)}'
-        return f'{api_url_base}/{type}/{quote(country)}/{quote(category)}'
-
-    link_api = getLinkApi(country, type, category)
-
-    try:
-        link_api += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-
-    try:
-        # print(link_api)
-        return fn.dataRequest(api_request=link_api, output_type=output_type)
-    except Exception as e:
-        print(e)
-        
-
-def getCmtTotalByType(country=None, type=None, output_type=None):
-    """
-        Get detailed information about Comtrade Country Total by Import or Exports
-        =================================================================================
-
-        Parameters:
-        -----------
-        country:string.
-                    for example:
-                    country = 'country_name' ,
-
-        type: string.
-                for example:
-                    type = 'import'
-                    type = 'export'
-
-        output_type: string.
-                    'dict'(default) for dictionary format output, 'df' for data frame,
-                    'raw' for list of dictionaries directly from the web.
-
-        Notes
-        -----
-        country and type parameters are not optional.
-
-        Example
-        -------
-        getCmtTotalByType(country = 'Portugal', type = 'import', output_type = None )
-
-        getCmtTotalByType(country = 'United States', type = 'export', output_type = 'raw' )
-
-        getCmtTotalByType(country = 'Brazil', type = import, output_type = 'df' )
-
-        """
-
-
-    if country is None:
-        return f'country is missing'
-
-    if type is None:
-        return f"type is missing. Choose 'import' or 'export'"
-
-    def getLinkApi(country, type):
-        api_url_base = "https://api.tradingeconomics.com/comtrade"
-
-        return f'{api_url_base}/{type}/{quote(country)}/totals/?c={glob.apikey}'
-
-    link_api = getLinkApi(country, type)
-
-    try:
-        # print(link_api)
-        return fn.dataRequest(api_request=link_api, output_type=output_type)
-    except Exception as e:
-        print(e)
-
-def getCmtCountryFilterByType(country1=None, country2=None, type=None, output_type=None):
-    """
-        Get detailed information about Comtrade Countries filter by type 'import' or 'export'
-        =================================================================================
-
-        Parameters:
-        -----------
-        country:string.
-                 for example:
-                    country1 = 'country_name'
-                    country2 = 'country_name'
-
-        type: string.
-                for example:
-                    type = 'import'
-                    type = 'export'
-        category: string.
-                for example:
-                    category = 'live animals'
-                    category = 'Swine, live'
-                    category = 'Sheep and goats, live'
-
-
-        output_type: string.
-                 'dict'(default) for dictionary format output, 'df' for data frame,
-                 'raw' for list of dictionaries directly from the web.
-
-        Notes
-        -----
-        'country1' and 'type' parameters are not optional.
-
-
-        Example
-        -------
-        getCmtCountryFilterByType(country1 = 'Portugal', country2 = 'Spain', type = 'import' )
-
-        getCmtCountryFilterByType(country1 = 'United States', type = 'export')
-
-
-        """
-
-    if country1 is None:
-        return f'country is missing'
-    if type is None:
-        return f"type is missing. Choose 'import' or 'export'"
-
-    def getLinkApi(country1, country2 ):
-        api_url_base = "https://api.tradingeconomics.com/comtrade/country"
-
-        if country2 is None:
-            return f'{api_url_base}/{quote(country1)}'
-        return f'{api_url_base}/{quote(country1)}/{quote(country2)}'
-
-    link_api = getLinkApi(country1, country2)
-
-    try:
-        link_api += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-
-    try:
-        link_api += f'&type={type}'
-
-    except AttributeError:
-        raise TypeError('type is missing. Choose "import" or "export"')
-
-    try:
-        # print(link_api)
-        return fn.dataRequest(api_request=link_api, output_type=output_type)
-    except Exception as e:
-        print(e)
-
-
-def getCmtSnapshotByType(country=None, type=None, output_type=None):
-    """
-        Get Snapshot of data per country filtered by type: import or export
-        =================================================================================
-
-        Parameters:
-        -----------
-        country:string.
-                    for example:
-                    country = 'country_name' ,
-
-        type: string.
-                for example:
-                    type = 'import'
-                    type = 'export'
-
-        output_type: string.
-                    'dict'(default) for dictionary format output, 'df' for data frame,
-                    'raw' for list of dictionaries directly from the web.
-
-        Notes
-        -----
-        country and type parameters are not optional.
-
-        Example
-        -------
-        getCmtSnapshotByType(country = 'Portugal', type = 'import', output_type = None )
-
-        getCmtSnapshotByType(country = 'United States', type = 'export', output_type = 'raw' )
-
-        getCmtSnapshotByType(country = 'Brazil', type = import, output_type = 'df' )
-
-        """
-
-
-    if country is None:
-        raise ParametersError (f'country is missing')
-
-    if type is None:
-        raise ParametersError (f"type is missing. Choose 'import' or 'export'")
-
-    def getLinkApi(country, type):
-        api_url_base = "https://api.tradingeconomics.com/comtrade/country"
-
-        return f'{api_url_base}/{quote(country)}?type={type}&c={glob.apikey}'
-
-    link_api = getLinkApi(country, type)
-
-    try:
-        # print(link_api)
-        return fn.dataRequest(api_request=link_api, output_type=output_type)
-    except Exception as e:
-        print(e)
+import json 
+import urllib 
+import pandas as pd
+import sys
+from datetime import *
+
+from . import functions as fn
+from . import glob
+import ssl
+
+PY3 = sys.version_info[0] == 3
+
+if PY3: # Python 3+
+    from urllib.request import urlopen
+    from urllib.parse import quote
+else: # Python 2.X
+    from urllib import urlopen
+    from urllib import quote
+
+
+class ParametersError(ValueError):
+    pass
+
+class CredentialsError(ValueError):
+    pass
+
+class LoginError(AttributeError):
+    pass
+
+class WebRequestError(ValueError):
+    pass
+
+class DateError(ValueError):
+    pass
+
+            
+def checkCountry(country):
+    linkAPI = 'https://api.tradingeconomics.com/country/'       
+    if type(country) is str:
+        linkAPI += quote(country.lower())
+    else:
+        linkAPI += quote(",".join(country), safe='')
+    return linkAPI
+
+def checkCountryRatings(country):
+    linkAPI = 'https://api.tradingeconomics.com/ratings/'       
+    if type(country) is str:
+        linkAPI += quote(country.lower())
+    else:
+        linkAPI += quote(",".join(country), safe='')
+    return linkAPI
+   
+def checkIndic(indicators, linkAPI):       
+    if type(indicators) is str:
+        linkAPI += '/' + quote(indicators, safe='')
+    else:
+        linkAPI += '/' + quote(",".join(indicators), safe='')
+    return linkAPI
+
+  
+
+def getResults(webResults, country):
+        names = ['country', 'category', 'title', 'latestvalue', 'latestvaluedate', 'source', 'unit', 'url', 'categorygroup', 'adjustment', 'frequency','historicaldatasymbol', 'createdate', 'previousvalue', 'previousvaluedate']
+        names2 = ['Country', 'Category', 'Title', 'LatestValue', 'LatestValueDate',  'Source', 'Unit', 'URL', 'CategoryGroup', 'Adjustment', 'Frequency', 'HistoricalDataSymbol', 'CreateDate', 'PreviousValue', 'PreviousValueDate']
+        maindf = pd.DataFrame() 
+        
+        for i in range(len(names)):
+            names[i] = [d[names2[i]]  for d in webResults]
+            maindf = pd.concat([maindf, pd.DataFrame(names[i], columns = [names2[i]])], axis = 1) 
+        maindf['Country'] =  maindf['Country'].map(lambda x: x.strip())
+        return maindf 
+
+
+
+def getUpdateResults(webResults, date):
+        names = ['country', 'category', 'historicalDataSymbol', 'lastUpdate']
+        names2 = ['Country', 'Category', 'HistoricalDataSymbol', 'LastUpdate']
+        maindf = pd.DataFrame() 
+        
+        for i in range(len(names)):
+            names[i] = [d[names2[i]]  for d in webResults]
+            maindf = pd.concat([maindf, pd.DataFrame(names[i], columns = [names2[i]])], axis = 1) 
+        maindf['date'] =  maindf['date'].map(lambda x: x.strip())
+        return maindf 
+
+
+
+def getIndicatorData(country = None, indicators = None, output_type = None):
+    """
+    Return a list of all indicators, indicators by country or country-indicator pair.
+    =================================================================================
+    Parameters:
+    -----------
+    country: string or list.
+             String for one country information. List of strings for 
+             several countrys, for example country = ['country_name', 'country_name'].
+    indicators: string or list.
+             String for one indicator. List of strings for several indicators, for example 
+             indicators = 'indicator_name' or 
+             indicators = ['indicator_name', 'indicator_name']
+    output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+    Notes
+    -----
+    All parameters are optional. Without parameters a list of all indicators will be provided. 
+    Example
+    -------
+    getIndicatorData(country = 'United States', indicators = 'Imports', output_type = 'df')
+    getIndicatorData(country = ['United States', 'Portugal'], indicators = ['Imports','Exports'])
+    """
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+    
+    if country == None:
+         linkAPI = 'https://api.tradingeconomics.com/indicators/'
+    else:
+         linkAPI = checkCountry(country)
+    
+    if indicators == None:
+         linkAPI = linkAPI
+    else:
+         linkAPI = checkIndic(indicators, linkAPI)
+
+    if indicators and country is None:
+        linkAPI = 'https://api.tradingeconomics.com/country/all'
+        linkAPI = checkIndic(indicators, linkAPI)
+
+    try:
+        linkAPI += '?c=' + glob.apikey
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+
+    try:
+        #print(linkAPI)
+        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
+    except Exception as e:
+        print(e)  
+ 
+def getRatings(country=None, rating = None, output_type='df'):
+    """
+    Return a list of all countrys by rating.
+    =================================================================================
+    Parameters:
+    -----------
+    country: string or list.
+             String for one country information. List of strings for 
+             several countrys, for example country = ['country_name', 'country_name'].
+        output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+    Notes
+    -----
+    All parameters are optional. Without parameters a list of all indicators will be provided. 
+    Example
+    -------
+    getRatings(country = 'United States', rating = None, output_type = 'df')
+    getRatings(country = ['United States', 'Portugal'], rating = None, output_type = 'df')
+    """
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+    
+    if country == None:
+        linkAPI = 'https://api.tradingeconomics.com/ratings'
+    else:
+        linkAPI = checkCountryRatings(country)
+
+    try:
+        linkAPI += '?c=' + glob.apikey
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+  
+    try:
+        #print(linkAPI)
+        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
+    except Exception as e:
+        print(e)
+
+
+
+def getDiscontinuedIndicator(country=None, output_type=None):
+    """
+    Returns a list of List of discontinued series for all countries, by country or multiple countries.
+    =================================================================================
+    Parameters:
+    -----------
+        country: string or list.
+                list of latest updates by initial date, for example:
+                country = 'china'
+                country = ['united states', 'china']          
+        output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+    Notes
+    -----
+    Without parameters a List of discontinued series for all countries will be provided. 
+    
+    Example
+    -------
+            getDiscontinuedIndicator()
+
+            getDiscontinuedIndicator(ountry = ['united states', 'china'], output_type = 'df')
+    """
+    
+    # d is a dictionary used for create the api url
+    d = {
+        'url_base': 'https://api.tradingeconomics.com/country',
+        'country': '/all',
+        'discontinued_tag' : '/discontinued',
+        'key': f'?c={glob.apikey}',
+        'output_type' : ''
+    }
+
+    if country:
+        d['country'] = f'/{fn.stringOrList(country)}'
+
+    api_url_request = "%s%s%s%s" % (d['url_base'], d['country'],d['discontinued_tag'],  d['key']) 
+    print(api_url_request)
+    return fn.dataRequest(api_request=api_url_request, output_type=output_type)
+
+
+def getIndicatorByCategoryGroup(country=None, category_group=None, output_type=None):
+    """
+    Returns a list of List of discontinued series for all countries, by country or multiple countries.
+    =================================================================================
+    Parameters:
+    -----------
+        country: string or list.
+                country = 'china'
+                country = ['united states', 'china']    
+        category_group: string or list.
+                category_group = 'gdp'
+                category_group = 'labour'
+                category_group = 'markets'
+
+        output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+    Notes
+    -----
+     
+    
+    Example
+    -------
+            getIndicatorByCategoryGroup(country = 'united states', category_group = 'gdp', output_type = 'df')
+
+            getIndicatorByCategoryGroup(country = ['united states', 'china'],category_group = 'markets', output_type = 'df')
+    """
+    
+    # d is a dictionary used for create the api url
+    d = {
+        'url_base': 'https://api.tradingeconomics.com/country',
+        'country': '',
+        'category_group' : '',
+        'key': f'?c={glob.apikey}',
+        'output_type' : ''
+    }
+
+    if country and category_group:
+        
+        
+        d['country'] = f'/{fn.stringOrList(country)}'
+        d['category_group']=f'&group={fn.stringOrList(category_group)}'
+        api_url_request = "%s%s%s%s" % (d['url_base'], d['country'],  d['key'], d['category_group']) 
+        #print(api_url_request)
+        return fn.dataRequest(api_request=api_url_request, output_type=output_type)
+         
+
+
+    return 'Country and category are required'
+
+
+def getIndicatorByTicker(ticker=None, output_type=None):
+    """
+    Returns a list of Specific indicator by ticker.
+    =================================================================================
+    Parameters:
+    -----------
+        ticker: string or list.
+                ticker = 'USURTOT'
+                ticker = ['WGDPCHIN', 'USURTOT']    
+        output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+    Notes
+    -----
+     
+    
+    Example
+    -------
+            getIndicatorByTicker(ticker = 'USURTOT', output_type = 'df')
+
+            getIndicatorByTicker(ticker = ['WGDPCHIN', 'USURTOT'], output_type = 'df')
+    """
+    
+    # d is a dictionary used for create the api url
+    d = {
+        'url_base': 'https://api.tradingeconomics.com/country',
+        'country': '/country',
+        'ticker' : '',
+        'key': f'?c={glob.apikey}',
+        'output_type' : ''
+    }
+
+    if ticker:
+        d['ticker']=f'/ticker/{fn.stringOrList(ticker)}'
+        api_url_request = "%s%s%s" % (d['url_base'], d['ticker'],  d['key']) 
+        #print(api_url_request)
+        return fn.dataRequest(api_request=api_url_request, output_type=output_type)
+        #return
+         
+
+    return 'Ticker is required'
+
+    
+def getLatestUpdates(country=None, init_date=None, time=None, output_type=None):
+    """
+    Returns Lastest Updates by country, by country and initial date, by initial date only or initial date and time.
+    =================================================================================
+    Parameters:
+    -----------
+        country: string or list.
+                country = 'united states'
+                country = ['united states', 'portugal']
+
+        init_date: string format (yyyy-mm-dd).
+                init_date = '2021-06-01'
+
+         time: string format (hh:mm).
+                time = '15:20'
+
+        output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+    Notes
+    -----
+    all parameters are optional.
+    
+    Example
+    -------
+            getLatestUpdates(country = 'united states', output_type = 'df')
+            getLatestUpdates(country = 'united states',init_date = '2021-06-01', output_type = 'df')
+            getLatestUpdates(country = ['united states','portugal'],init_date = '2021-06-01', output_type = 'df')
+            getLatestUpdates(init_date = '2021-10-18', time='15:20', output_type = 'df')
+    """
+    
+    # d is a dictionary used for create the api url
+    d = {
+        'url_base': 'https://api.tradingeconomics.com/updates',
+        'country': '',
+        'ticker' : '',
+        'time' : '',
+        'init_date': '',
+        'key': f'?c={glob.apikey}',
+        'output_type' : ''
+    }
+    if init_date :        
+        try: 
+            fn.validate(init_date)
+            d['init_date']=f'/{init_date}'
+        except ValueError:
+            raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
+        if time:
+            try:
+                fn.timeValidate(time)
+                d['time']=f'&time={time}'     
+            except ValueError:
+                raise DateError ('Incorrect time format, should be HH:MM.')
+
+    if country:
+        d['country']=f'/country/{fn.stringOrList(country)}'
+
+        
+    
+    api_url_request = "%s%s%s%s%s" % (d['url_base'], d['country'],  d['init_date'],  d['key'],  d['time']) 
+    print(api_url_request)
+    return fn.dataRequest(api_request=api_url_request, output_type=output_type)
+
+         
+def getPeers(country=None, category=None, ticker=None, output_type=None):
+    """
+    Returns indicators peers by country, by category and ticker.
+    =================================================================================
+    Parameters:
+    -----------
+        country: string
+        category: string
+        ticker; stirng
+
+        output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+    
+    Example
+    -------
+            getPeers(ticker ='CPI YOY', output_type = 'df')
+            getPeers(country ='united states', output_type = 'df')
+            getPeers(country ='united states', category ='money', output_type = 'df')
+    """
+   
+    # d is a dictionary used for create the api url
+    d = {
+        'url_base': 'https://api.tradingeconomics.com/peers/',
+        'country': '',
+        'ticker' : '',
+        'category': '',
+        'key': f'?c={glob.apikey}',
+        'output_type' : ''
+    }
+
+    if country:
+        country = country.replace(' ', '%20')
+        d['country']=f'country/{country}'
+        if not(category is None):
+            d['category']=f'/{category}'
+    
+    if ticker:
+       d['ticker']=ticker.replace(' ', '%20')
+        
+    
+    api_url_request = "%s%s%s%s%s" % (d['url_base'],d['ticker'], d['country'],  d['category'],  d['key']) 
+    print(api_url_request)
+    return fn.dataRequest(api_request=api_url_request, output_type=output_type)
+
+    
+def getAllCountries(output_type=None):
+    """
+    Return a list of countries.
+    =================================================================================
+    Parameters:
+    -----------
+    output_type parameter can be 'df' or 'raw'
+    Example
+    -------
+    getAllCountries()
+    getAllCountries(out_type='df')
+    """
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+    
+    linkAPI = 'https://api.tradingeconomics.com/country/'
+
+    try:
+        linkAPI += '?c=' + glob.apikey
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+
+    try:
+        #print(linkAPI)
+        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
+    except Exception as e:
+        print(e)
```

### Comparing `tradingeconomics-4.2.8/tradingeconomics/federalReserve.py` & `tradingeconomics-4.2.9/tradingeconomics/federalReserve.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,385 +1,385 @@
-import json
-import itertools
-import urllib 
-import pandas as pd
-import sys
-from datetime import *
-from dateutil.relativedelta import relativedelta
-from . import functions as fn
-from . import glob
-import ssl
-
-PY3 = sys.version_info[0] == 3
-
-if PY3: # Python 3+
-    from urllib.request import urlopen
-    from urllib.parse import quote
-else: # Python 2.X
-    from urllib import urlopen
-    from urllib import quote
-
-class ParametersError(ValueError):
-    pass
-
-class DateError(ValueError):
-    pass
-
-class CredentialsError(ValueError):
-    pass
-
-class LoginError(AttributeError):
-    pass
-
-class WebRequestError(ValueError):
-    pass
-
-def checkFedRSymbol(linkAPI, symbol):
-    linkAPI = 'https://api.tradingeconomics.com/fred/snapshot/symbol/'     
-    if symbol != None:
-        if type(symbol) == str:
-            linkAPI +=  quote(symbol)
-        else:    
-            linkAPI += quote("/".join(symbol), safe='')
-     
-    return linkAPI
-
-def checkFedRCountry(linkAPI, country):
-    linkAPI = 'https://api.tradingeconomics.com/fred/snapshot/country/'     
-    if country != None:
-        if type(country) == str:
-            linkAPI +=  quote(country)
-        else:    
-            linkAPI += quote("/".join(country), safe='')
-     
-    return linkAPI
-
-def checkFedRState(linkAPI, state):
-    linkAPI = 'https://api.tradingeconomics.com/fred/snapshot/state/'     
-    if state != None:
-        if type(state) == str:
-            linkAPI +=  quote(state)
-        else:    
-            linkAPI += quote("/".join(state), safe='')
-     
-    return linkAPI
-
-def checkFedRCounty(linkAPI, county):
-    linkAPI = 'https://api.tradingeconomics.com/fred/snapshot/county/'     
-    if county != None:
-        if type(county) == str:
-            linkAPI +=  quote(county)
-        else:    
-            linkAPI += quote("/".join(county), safe='') 
-     
-    return linkAPI
-
-def checkFedRPage(linkAPI, page_number):
-    if page_number != None:
-        linkAPI +=  '/{0}'.format(page_number) 
-    
-    return linkAPI
-
-
-def getFedRStates(county = None, output_type = None):
-    """
-    List of all US states and list of all counties per state.
-    =================================================================================
-
-    Parameters:
-    -----------
-    name:list.
-             List of strings of all US states.
-    county:string.            
-            List of all counties per state. 
-                for example:
-                county = 'arkansas'             
-    output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web. 
-
-    Notes
-    -----
-    For all states no parameters are required. 
-
-    Example
-    -------
-    getFedRStates(county = None, output_type = None)
-
-    getFedRStates(county = 'arkansas', output_type = None)
-    """
-    name = ""          
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-    
-    linkAPI = 'https://api.tradingeconomics.com/fred/states'
-
-    if county != None:
-        linkAPI = 'https://api.tradingeconomics.com/fred/counties/' + quote("".join(county))
-    
-    if name == None and county == None:
-        linkAPI = 'https://api.tradingeconomics.com/fred/states'  
-        
-    try:
-        linkAPI += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-
-   
-    try:
-        #print(linkAPI)
-        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
-    except Exception as e:
-        print(e)
-
-
-def getFedRSnaps(symbol = None, url = None, country = None, state = None, county = None, page_number = None, output_type = None):
-    """
-    Snapshots can be accessed through symbol, url, country, state or county. All have pagination.
-    =================================================================================
-
-    Parameters:
-    -----------
-    symbol:list or string.
-             snapshots of sepecific symbol or list of snapshots of symbols.
-             for example:
-                 symbol = None
-                 symbol = 'te_symbol'
-    url:string.
-             String of a specific url, for example:
-                 url = 'specific url'
-    country:list.
-             In this case only a list of US will be provided.
-                 country = 'united states'
-    state:list.
-             A list of states or one state, for example:
-                 state = 'state_name'
-                 state = ['state_name', 'state_name']
-    county:list.            
-             A list of counties or county, for example:
-                  county = 'county_name' 
-                  county = 'pike county, ar'
-                  county = ['county_name', 'county_name' ]                     
-    output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web. 
-
-    Notes
-    -----
-    At least one of the parameters must be provided. All have pagination 
-
-    Example
-    -------
-    getFedRSnaps(symbol = 'ALLMARGATTN', url = None, country = None, state = None, county = None, output_type = None)
-
-    getFedRSnaps(symbol = None, url = 'united states''/united-states/white-to-non-white-racial-dissimilarity-index-for-benton-county-ar-fed-data.html', country = None, state = None, county = None, page_number = None, output_type = None)
-  
-    getFedRSnaps(symbol = None, url = None, country = 'united states', state = None, county = None, output_type = None)
-
-    getFedRSnaps(symbol = None, url = None, country = None, state = 'tennessee', county = None, output_type = None)
-
-    getFedRSnaps(symbol = None, url = None, country = None, state = None, county = 'arkansas', output_type = None)
-  
-    """
- 
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-
-    linkAPI = 'https://api.tradingeconomics.com/fred/snapshot/'
-
-    if symbol != None: 
-        linkAPI = checkFedRSymbol(linkAPI, symbol) 
-    elif url != None:    
-        linkAPI = 'https://api.tradingeconomics.com/fred/snapshot/url/'+ '?c=' + glob.apikey + '&url=' + quote(str(url))      
-    elif country != None:    
-        linkAPI = checkFedRCountry(linkAPI, country)  
-    elif state != None:   
-        linkAPI = checkFedRState(linkAPI, state) 
-    elif county != None:  
-        linkAPI = checkFedRCounty(linkAPI, county)    
-    else:                
-        return "A parameter must be provided!"
-    
-    if page_number != None:
-        linkAPI = checkFedRPage(linkAPI, page_number) +'?c=' + glob.apikey  
-    else:  
-        linkAPI += '?c=' + glob.apikey
-    
-    try:
-        #print(linkAPI)
-        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
-    except Exception as e:
-        print(e)
-
-def getFedRCountyOld(state=None,county=None, output_type = None):
-    """
-    List of Pike County, AR.
-    =================================================================================
-
-    Parameters:
-    -----------
-    county:list.
-             List of strings of all Pike County categories.
-             
-    output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web. 
-    Notes:
-    ------
-    No parameters are required, because it can only be Pike County.
-
-    Example
-    -------
-    getFedRCounty(output_type = None)
-
-    """
-             
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-    
-    
-    linkAPI = 'https://api.tradingeconomics.com/fred/snapshot/county/Pike%20County,%20AR'
-     
-    try:
-        linkAPI += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-
-    
-    try:
-        #print(linkAPI)
-        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
-    except Exception as e:
-        print(e)     
-
-def getFedRCounty(state=None,county=None, output_type = None):
-    """
-    List of state's counties or list of counties indicators
-    =================================================================================
-
-    Parameters:
-    -----------
-
-    state:string.
-            string with state name (example: "Nevada" ).
-    county:string.
-            string with county name (example: "Pike County, AR" ).
-            
-    output_type: string.
-            'dict'(default) for dictionary format output, 'df' for data frame,
-            'raw' for list of dictionaries directly from the web. 
-    Notes:
-    ------
-    
-
-    Example
-    -------
-    getFedRCounty(state='nevada',output_type = None)
-    getFedRCounty(county='Pike County, AR',output_type = None)
-
-    """
-            
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-    
-    # d is a dictionary used for create the api url
-    d = {
-        'url_base': 'https://api.tradingeconomics.com/fred/snapshot/county/',
-        'state': '',
-        'county' : '',
-        'key': f'?c={glob.apikey}',
-        'output_type' : ''
-    }
-
-    if state:
-        d['state'] = quote(state)
-    if county:
-        d['county'] = quote(county)
-
-    api_url_request = "%s%s%s%s" % (d['url_base'], d['state'], d['county'],  d['key'])
-    return fn.dataRequest(api_request=api_url_request, output_type=output_type)
-       
-
-
-def getFedRHistorical(symbol = None, initDate=None,endDate=None, output_type = None):
-    """
-    Get Historical data.
-    =================================================================================
-
-    Parameters:
-    -----------
-    symbol:list.
-             List of strings by a specific symbol or symbols.
-             for example:
-                symbol = 'racedisparity005007'
-                symbol = ['racedisparity005007', '2020ratio002013']  
-    initDate: string.
-            initDate = '2018-05-01'
-    endDate: string.
-            endDate = '2018-06-01'    
-    output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web. 
-    
-    Notes
-    -----
-    A symbol is required. 
-
-    Example
-    -------
-    getFedRHistorical(symbol = 'racedisparity005007', output_type = 'df')
-
-    getFedRHistorical(symbol = ['racedisparity005007', '2020ratio002013'], output_type = 'df')
-
-    getFedRHistorical(symbol=['racedisparity005007', '2020ratio002013'],initDate='2018-05-01',output_type='df')
-
-    getFedRHistorical(symbol=['racedisparity005007', '2020ratio002013'],initDate='2017-05-01', endDate='2019-01-01',output_type='df')
-
-    
-    """
-
-
-    # d is a dictionary used for create the api url
-    d = {
-        'url_base': 'https://api.tradingeconomics.com/fred/historical',
-        'symbol': '',
-        'initDate': '',
-        'endDate':'',
-        'key': f'?c={glob.apikey}',
-        'output_type' : ''
-    }
-
-    if initDate:     
-        fn.validate(initDate)
-        d['initDate']=f'&d1={initDate}'
-        
-    if endDate:
-        fn.validate(endDate)
-        d['endDate']=f'&d2={endDate}'
-        fn.validatePeriod(initDate, endDate)
-        
-
-    if symbol:
-        d['symbol'] = f'/{fn.stringOrList(symbol)}'
-        
-    
-    api_url_request = "%s%s%s%s%s" % (d['url_base'], d['symbol'],  d['key'],d['initDate'],d['endDate']) 
-    # print(api_url_request)
-    response = fn.dataRequest(api_request=api_url_request, output_type=output_type)
-    return response
+import json
+import itertools
+import urllib 
+import pandas as pd
+import sys
+from datetime import *
+from dateutil.relativedelta import relativedelta
+from . import functions as fn
+from . import glob
+import ssl
+
+PY3 = sys.version_info[0] == 3
+
+if PY3: # Python 3+
+    from urllib.request import urlopen
+    from urllib.parse import quote
+else: # Python 2.X
+    from urllib import urlopen
+    from urllib import quote
+
+class ParametersError(ValueError):
+    pass
+
+class DateError(ValueError):
+    pass
+
+class CredentialsError(ValueError):
+    pass
+
+class LoginError(AttributeError):
+    pass
+
+class WebRequestError(ValueError):
+    pass
+
+def checkFedRSymbol(linkAPI, symbol):
+    linkAPI = 'https://api.tradingeconomics.com/fred/snapshot/symbol/'     
+    if symbol != None:
+        if type(symbol) == str:
+            linkAPI +=  quote(symbol)
+        else:    
+            linkAPI += quote("/".join(symbol), safe='')
+     
+    return linkAPI
+
+def checkFedRCountry(linkAPI, country):
+    linkAPI = 'https://api.tradingeconomics.com/fred/snapshot/country/'     
+    if country != None:
+        if type(country) == str:
+            linkAPI +=  quote(country)
+        else:    
+            linkAPI += quote("/".join(country), safe='')
+     
+    return linkAPI
+
+def checkFedRState(linkAPI, state):
+    linkAPI = 'https://api.tradingeconomics.com/fred/snapshot/state/'     
+    if state != None:
+        if type(state) == str:
+            linkAPI +=  quote(state)
+        else:    
+            linkAPI += quote("/".join(state), safe='')
+     
+    return linkAPI
+
+def checkFedRCounty(linkAPI, county):
+    linkAPI = 'https://api.tradingeconomics.com/fred/snapshot/county/'     
+    if county != None:
+        if type(county) == str:
+            linkAPI +=  quote(county)
+        else:    
+            linkAPI += quote("/".join(county), safe='') 
+     
+    return linkAPI
+
+def checkFedRPage(linkAPI, page_number):
+    if page_number != None:
+        linkAPI +=  '/{0}'.format(page_number) 
+    
+    return linkAPI
+
+
+def getFedRStates(county = None, output_type = None):
+    """
+    List of all US states and list of all counties per state.
+    =================================================================================
+
+    Parameters:
+    -----------
+    name:list.
+             List of strings of all US states.
+    county:string.            
+            List of all counties per state. 
+                for example:
+                county = 'arkansas'             
+    output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+
+    Notes
+    -----
+    For all states no parameters are required. 
+
+    Example
+    -------
+    getFedRStates(county = None, output_type = None)
+
+    getFedRStates(county = 'arkansas', output_type = None)
+    """
+    name = ""          
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+    
+    linkAPI = 'https://api.tradingeconomics.com/fred/states'
+
+    if county != None:
+        linkAPI = 'https://api.tradingeconomics.com/fred/counties/' + quote("".join(county))
+    
+    if name == None and county == None:
+        linkAPI = 'https://api.tradingeconomics.com/fred/states'  
+        
+    try:
+        linkAPI += '?c=' + glob.apikey
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+
+   
+    try:
+        #print(linkAPI)
+        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
+    except Exception as e:
+        print(e)
+
+
+def getFedRSnaps(symbol = None, url = None, country = None, state = None, county = None, page_number = None, output_type = None):
+    """
+    Snapshots can be accessed through symbol, url, country, state or county. All have pagination.
+    =================================================================================
+
+    Parameters:
+    -----------
+    symbol:list or string.
+             snapshots of sepecific symbol or list of snapshots of symbols.
+             for example:
+                 symbol = None
+                 symbol = 'te_symbol'
+    url:string.
+             String of a specific url, for example:
+                 url = 'specific url'
+    country:list.
+             In this case only a list of US will be provided.
+                 country = 'united states'
+    state:list.
+             A list of states or one state, for example:
+                 state = 'state_name'
+                 state = ['state_name', 'state_name']
+    county:list.            
+             A list of counties or county, for example:
+                  county = 'county_name' 
+                  county = 'pike county, ar'
+                  county = ['county_name', 'county_name' ]                     
+    output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+
+    Notes
+    -----
+    At least one of the parameters must be provided. All have pagination 
+
+    Example
+    -------
+    getFedRSnaps(symbol = 'ALLMARGATTN', url = None, country = None, state = None, county = None, output_type = None)
+
+    getFedRSnaps(symbol = None, url = 'united states''/united-states/white-to-non-white-racial-dissimilarity-index-for-benton-county-ar-fed-data.html', country = None, state = None, county = None, page_number = None, output_type = None)
+  
+    getFedRSnaps(symbol = None, url = None, country = 'united states', state = None, county = None, output_type = None)
+
+    getFedRSnaps(symbol = None, url = None, country = None, state = 'tennessee', county = None, output_type = None)
+
+    getFedRSnaps(symbol = None, url = None, country = None, state = None, county = 'arkansas', output_type = None)
+  
+    """
+ 
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+
+    linkAPI = 'https://api.tradingeconomics.com/fred/snapshot/'
+
+    if symbol != None: 
+        linkAPI = checkFedRSymbol(linkAPI, symbol) 
+    elif url != None:    
+        linkAPI = 'https://api.tradingeconomics.com/fred/snapshot/url/'+ '?c=' + glob.apikey + '&url=' + quote(str(url))      
+    elif country != None:    
+        linkAPI = checkFedRCountry(linkAPI, country)  
+    elif state != None:   
+        linkAPI = checkFedRState(linkAPI, state) 
+    elif county != None:  
+        linkAPI = checkFedRCounty(linkAPI, county)    
+    else:                
+        return "A parameter must be provided!"
+    
+    if page_number != None:
+        linkAPI = checkFedRPage(linkAPI, page_number) +'?c=' + glob.apikey  
+    else:  
+        linkAPI += '?c=' + glob.apikey
+    
+    try:
+        #print(linkAPI)
+        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
+    except Exception as e:
+        print(e)
+
+def getFedRCountyOld(state=None,county=None, output_type = None):
+    """
+    List of Pike County, AR.
+    =================================================================================
+
+    Parameters:
+    -----------
+    county:list.
+             List of strings of all Pike County categories.
+             
+    output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+    Notes:
+    ------
+    No parameters are required, because it can only be Pike County.
+
+    Example
+    -------
+    getFedRCounty(output_type = None)
+
+    """
+             
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+    
+    
+    linkAPI = 'https://api.tradingeconomics.com/fred/snapshot/county/Pike%20County,%20AR'
+     
+    try:
+        linkAPI += '?c=' + glob.apikey
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+
+    
+    try:
+        #print(linkAPI)
+        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
+    except Exception as e:
+        print(e)     
+
+def getFedRCounty(state=None,county=None, output_type = None):
+    """
+    List of state's counties or list of counties indicators
+    =================================================================================
+
+    Parameters:
+    -----------
+
+    state:string.
+            string with state name (example: "Nevada" ).
+    county:string.
+            string with county name (example: "Pike County, AR" ).
+            
+    output_type: string.
+            'dict'(default) for dictionary format output, 'df' for data frame,
+            'raw' for list of dictionaries directly from the web. 
+    Notes:
+    ------
+    
+
+    Example
+    -------
+    getFedRCounty(state='nevada',output_type = None)
+    getFedRCounty(county='Pike County, AR',output_type = None)
+
+    """
+            
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+    
+    # d is a dictionary used for create the api url
+    d = {
+        'url_base': 'https://api.tradingeconomics.com/fred/snapshot/county/',
+        'state': '',
+        'county' : '',
+        'key': f'?c={glob.apikey}',
+        'output_type' : ''
+    }
+
+    if state:
+        d['state'] = quote(state)
+    if county:
+        d['county'] = quote(county)
+
+    api_url_request = "%s%s%s%s" % (d['url_base'], d['state'], d['county'],  d['key'])
+    return fn.dataRequest(api_request=api_url_request, output_type=output_type)
+       
+
+
+def getFedRHistorical(symbol = None, initDate=None,endDate=None, output_type = None):
+    """
+    Get Historical data.
+    =================================================================================
+
+    Parameters:
+    -----------
+    symbol:list.
+             List of strings by a specific symbol or symbols.
+             for example:
+                symbol = 'racedisparity005007'
+                symbol = ['racedisparity005007', '2020ratio002013']  
+    initDate: string.
+            initDate = '2018-05-01'
+    endDate: string.
+            endDate = '2018-06-01'    
+    output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+    
+    Notes
+    -----
+    A symbol is required. 
+
+    Example
+    -------
+    getFedRHistorical(symbol = 'racedisparity005007', output_type = 'df')
+
+    getFedRHistorical(symbol = ['racedisparity005007', '2020ratio002013'], output_type = 'df')
+
+    getFedRHistorical(symbol=['racedisparity005007', '2020ratio002013'],initDate='2018-05-01',output_type='df')
+
+    getFedRHistorical(symbol=['racedisparity005007', '2020ratio002013'],initDate='2017-05-01', endDate='2019-01-01',output_type='df')
+
+    
+    """
+
+
+    # d is a dictionary used for create the api url
+    d = {
+        'url_base': 'https://api.tradingeconomics.com/fred/historical',
+        'symbol': '',
+        'initDate': '',
+        'endDate':'',
+        'key': f'?c={glob.apikey}',
+        'output_type' : ''
+    }
+
+    if initDate:     
+        fn.validate(initDate)
+        d['initDate']=f'&d1={initDate}'
+        
+    if endDate:
+        fn.validate(endDate)
+        d['endDate']=f'&d2={endDate}'
+        fn.validatePeriod(initDate, endDate)
+        
+
+    if symbol:
+        d['symbol'] = f'/{fn.stringOrList(symbol)}'
+        
+    
+    api_url_request = "%s%s%s%s%s" % (d['url_base'], d['symbol'],  d['key'],d['initDate'],d['endDate']) 
+    # print(api_url_request)
+    response = fn.dataRequest(api_request=api_url_request, output_type=output_type)
+    return response
     # return
```

### Comparing `tradingeconomics-4.2.8/tradingeconomics/financials.py` & `tradingeconomics-4.2.9/tradingeconomics/financials.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,213 +1,213 @@
-import urllib
-import sys
-from datetime import *
-from . import glob
-from . import functions as fn
-
-PY3 = sys.version_info[0] == 3
-
-if PY3:  # Python 3+
-    from urllib.request import urlopen
-    from urllib.parse import quote
-else:  # Python 2.X
-    from urllib import urlopen
-    from urllib import quote
-
-
-class ParametersError(ValueError):
-    pass
-
-
-class CredentialsError(ValueError):
-    pass
-
-
-class LoginError(AttributeError):
-    pass
-
-
-class DateError(ValueError):
-    pass
-
-
-class WebRequestError(ValueError):
-    pass
-
-
-def getFinancialsData(symbol = None, country = None, output_type=None):
-    """
-    Returns financial data and stocks fundamental information.
-    ==========================================================
-
-    Parameters:
-    -----------
-    symbols: string or list.
-             String to get data for symbol. List of strings to get data for
-             several symbols.
-    country: string or list.
-             String to get data for country. List of strings to get data for
-             several symbols.
-    output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web.
-
-    Example
-    -------
-    If no argument is provided, returns a list of all companies.
-            getFinancialsData()
-    To get companies financial data by symbol:
-            getFinancialsData(symbol='aapl:us', output_type='df')
-            
-            or
-            
-            getFinancialsData(symbol=['aapl:us','msft:us'], output_type='df')
-    To get companies by country:
-            getFinancialsData(country='united states', output_type='df')
-            
-            getFinancialsData(country=['united states', 'china'], output_type='df')
-    """
-
-    try:
-        # d is a dictionary used for create the api url
-        d = {
-            'url_base': 'https://api.tradingeconomics.com/financials',
-            'symbol': '',
-            'country': '/companies',
-            'key': f'?c={glob.apikey}',
-            'output_type' : ''
-        }
-    except AttributeError:
-        return "You are not logged in. Run te.login('guest:guest') to login"
-
-    if country and symbol:
-        return 'Cannot pass country and symbol arguments at the same time.'
-
-    if country:
-        #the 'key' value has to be changed due to url enpoint use of '?' or '&' characters. 
-        d['key']=f'&c={glob.apikey}'
-        d['country'] = f'/companies?country={fn.stringOrList(country)}'
-    elif symbol:
-        d['key']=f'&c={glob.apikey}'
-        d['country'] = ''
-        d['symbol'] = f'/symbol/{fn.stringOrList(symbol)}?'
-
-    
-    api_url_request = "%s%s%s%s" % (d['url_base'], d['symbol'],d['country'],  d['key']) 
-
-    return fn.dataRequest(api_request=api_url_request, output_type=output_type)
-
-
-def getFinancialsCategoryList(output_type=None):
-    """
-    Returns list of categories of financial data.
-    ==========================================================
-
-    Parameters:
-    -----------
-    output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web.
-
-    Example
-    -------
-    If no argument is provided, returns a list of all categories as a dictionary.
-    getFinancialsCategories()
-    getFinancialsCategories(output_type='df')
-    """
-
-    try:
-
-        d = {
-            'url_base': 'https://api.tradingeconomics.com/financials/categories',
-            'key': f'?c={glob.apikey}',
-            'output_type' : ''
-        }
-    except AttributeError:
-        return "You are not logged in. Run te.login('guest:guest') to login"
-
-    api_url_request = "%s%s" % (d['url_base'], d['key'])
-
-    return fn.dataRequest(api_request=api_url_request, output_type=output_type)
-
-
-
-def getFinancialsDataByCategory(category=None, output_type=None):
-
-    """
-    Returns financial data by categories.
-    ==========================================================
-
-    Parameters:
-    -----------
-    category: string or list.
-             String to get data for category. List of strings to get data for
-             several categories.
-    output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web.
-
-    Example
-    -------
-    Get data by financial categories:
-            getFinancialsDataByCategory(category='assets', output_type='df')
-            
-            or
-            
-            getFinancialsDataCategory(symbol=['assets','debt'], output_type='df')
-    """
-
-    try:
-        # d is a dictionary used for create the api url
-        d = {
-            'url_base': 'https://api.tradingeconomics.com/financials/category',
-            'symbol': f'/{category}',
-            'key': f'?c={glob.apikey}',
-            'output_type' : ''
-        }
-    except AttributeError:
-        return "You are not logged in. Run te.login('guest:guest') to login"
-    
-    if category:
-        #the 'key' value has to be changed due to url enpoint use of '?' or '&' characters. 
-        d['category'] = f'/{category}'
-    else:
-        return 'No category supplied'
-
-
-    api_url_request = "%s%s%s" % (d['url_base'], d['category'], d['key'])
-
-    return fn.dataRequest(api_request=api_url_request, output_type=output_type)
-
-
-def getSectors(output_type=None):
-    """
-    Returns all sectors.
-    ==========================================================
-
-    Parameters:
-    -----------
-
-    output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web. 
-    
-    Example
-    -------
-    Get data by financial categories:
-            getSectors()
-
-    """
-
-    linkAPI = 'https://api.tradingeconomics.com/sectors/'
-
-    try:
-        linkAPI += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-        
-    linkAPI = fn.checkDates(linkAPI)
-    
-    try:
-        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
-    except Exception as e:
+import urllib
+import sys
+from datetime import *
+from . import glob
+from . import functions as fn
+
+PY3 = sys.version_info[0] == 3
+
+if PY3:  # Python 3+
+    from urllib.request import urlopen
+    from urllib.parse import quote
+else:  # Python 2.X
+    from urllib import urlopen
+    from urllib import quote
+
+
+class ParametersError(ValueError):
+    pass
+
+
+class CredentialsError(ValueError):
+    pass
+
+
+class LoginError(AttributeError):
+    pass
+
+
+class DateError(ValueError):
+    pass
+
+
+class WebRequestError(ValueError):
+    pass
+
+
+def getFinancialsData(symbol = None, country = None, output_type=None):
+    """
+    Returns financial data and stocks fundamental information.
+    ==========================================================
+
+    Parameters:
+    -----------
+    symbols: string or list.
+             String to get data for symbol. List of strings to get data for
+             several symbols.
+    country: string or list.
+             String to get data for country. List of strings to get data for
+             several symbols.
+    output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web.
+
+    Example
+    -------
+    If no argument is provided, returns a list of all companies.
+            getFinancialsData()
+    To get companies financial data by symbol:
+            getFinancialsData(symbol='aapl:us', output_type='df')
+            
+            or
+            
+            getFinancialsData(symbol=['aapl:us','msft:us'], output_type='df')
+    To get companies by country:
+            getFinancialsData(country='united states', output_type='df')
+            
+            getFinancialsData(country=['united states', 'china'], output_type='df')
+    """
+
+    try:
+        # d is a dictionary used for create the api url
+        d = {
+            'url_base': 'https://api.tradingeconomics.com/financials',
+            'symbol': '',
+            'country': '/companies',
+            'key': f'?c={glob.apikey}',
+            'output_type' : ''
+        }
+    except AttributeError:
+        return "You are not logged in. Run te.login('guest:guest') to login"
+
+    if country and symbol:
+        return 'Cannot pass country and symbol arguments at the same time.'
+
+    if country:
+        #the 'key' value has to be changed due to url enpoint use of '?' or '&' characters. 
+        d['key']=f'&c={glob.apikey}'
+        d['country'] = f'/companies?country={fn.stringOrList(country)}'
+    elif symbol:
+        d['key']=f'&c={glob.apikey}'
+        d['country'] = ''
+        d['symbol'] = f'/symbol/{fn.stringOrList(symbol)}?'
+
+    
+    api_url_request = "%s%s%s%s" % (d['url_base'], d['symbol'],d['country'],  d['key']) 
+
+    return fn.dataRequest(api_request=api_url_request, output_type=output_type)
+
+
+def getFinancialsCategoryList(output_type=None):
+    """
+    Returns list of categories of financial data.
+    ==========================================================
+
+    Parameters:
+    -----------
+    output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web.
+
+    Example
+    -------
+    If no argument is provided, returns a list of all categories as a dictionary.
+    getFinancialsCategories()
+    getFinancialsCategories(output_type='df')
+    """
+
+    try:
+
+        d = {
+            'url_base': 'https://api.tradingeconomics.com/financials/categories',
+            'key': f'?c={glob.apikey}',
+            'output_type' : ''
+        }
+    except AttributeError:
+        return "You are not logged in. Run te.login('guest:guest') to login"
+
+    api_url_request = "%s%s" % (d['url_base'], d['key'])
+
+    return fn.dataRequest(api_request=api_url_request, output_type=output_type)
+
+
+
+def getFinancialsDataByCategory(category=None, output_type=None):
+
+    """
+    Returns financial data by categories.
+    ==========================================================
+
+    Parameters:
+    -----------
+    category: string or list.
+             String to get data for category. List of strings to get data for
+             several categories.
+    output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web.
+
+    Example
+    -------
+    Get data by financial categories:
+            getFinancialsDataByCategory(category='assets', output_type='df')
+            
+            or
+            
+            getFinancialsDataCategory(symbol=['assets','debt'], output_type='df')
+    """
+
+    try:
+        # d is a dictionary used for create the api url
+        d = {
+            'url_base': 'https://api.tradingeconomics.com/financials/category',
+            'symbol': f'/{category}',
+            'key': f'?c={glob.apikey}',
+            'output_type' : ''
+        }
+    except AttributeError:
+        return "You are not logged in. Run te.login('guest:guest') to login"
+    
+    if category:
+        #the 'key' value has to be changed due to url enpoint use of '?' or '&' characters. 
+        d['category'] = f'/{category}'
+    else:
+        return 'No category supplied'
+
+
+    api_url_request = "%s%s%s" % (d['url_base'], d['category'], d['key'])
+
+    return fn.dataRequest(api_request=api_url_request, output_type=output_type)
+
+
+def getSectors(output_type=None):
+    """
+    Returns all sectors.
+    ==========================================================
+
+    Parameters:
+    -----------
+
+    output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+    
+    Example
+    -------
+    Get data by financial categories:
+            getSectors()
+
+    """
+
+    linkAPI = 'https://api.tradingeconomics.com/sectors/'
+
+    try:
+        linkAPI += '?c=' + glob.apikey
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+        
+    linkAPI = fn.checkDates(linkAPI)
+    
+    try:
+        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
+    except Exception as e:
         print(e)
```

### Comparing `tradingeconomics-4.2.8/tradingeconomics/forecasts.py` & `tradingeconomics-4.2.9/tradingeconomics/forecasts.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-import json 
-import urllib 
-import pandas as pd
-from datetime import *
-import sys
-from . import functions as fn
-from . import glob
-import ssl
-
-PY3 = sys.version_info[0] == 3
-
-if PY3: # Python 3+
-    from urllib.request import urlopen
-    from urllib.parse import quote
-else: # Python 2.X
-    from urllib import urlopen
-    from urllib import quote
-      
-
-class ParametersError(ValueError):
-    pass
-
-class CredentialsError(ValueError):
-    pass
-
-class LoginError(AttributeError):
-    pass
-  
-class WebRequestError(ValueError):
-    pass
-  
-def checkCountry(country):
-    linkAPI = 'https://api.tradingeconomics.com/forecast/country/'       
-    if type(country) is str:
-        linkAPI += quote(country, safe='')
-    else:
-        #multiCountry = ",".join(country)
-        linkAPI += quote(",".join(country), safe='')
-    return linkAPI
-        
-def checkIndic(indicator):
-    linkAPI = 'https://api.tradingeconomics.com/forecast/indicator/'        
-    if type(indicator) is str:
-        linkAPI += quote(indicator, safe='')
-    else:
-        #multiIndic = ",".join(indicator)
-        linkAPI += quote(",".join(indicator), safe='')
-    return linkAPI
-
-def getLink(country, indicator):
-    linkAPI = 'https://api.tradingeconomics.com/forecast/country/'
-    if type(country) is str:
-        linkAPI += quote(country)
-    else:
-        #multiCountry = ",".join(country)
-        linkAPI += quote(",".join(country), safe='') 
-    if type(indicator) is str:
-        linkAPI += '/indicator/' + quote(indicator, safe='')
-    else:
-        #multiIndic = ",".join(indicator)
-        linkAPI += '/indicator/' + quote(",".join(indicator), safe='') 
-    return linkAPI
-
-    
-def getForecastData(country = None, indicator = None, output_type = None):
-    """
-     Return forecast values by country, by indicator, by country and indicator.
-    ===========================================================================
-
-    Parameters:
-    -----------
-    country: string or list.
-             String to get data for one country. List of strings to get data for
-             several countries. For example, country = ['United States', 'Australia'].
-    indicator: string or list.
-             String  to get data for one category. List of strings to get data for several calendar events.
-             For example, category = 'GDP Growth Rate' or 
-             category = ['Exports', 'Imports']
-    output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries without any parsing.  
-
-    Notes
-    -----
-    At least one of parameters, country or indicator, should be provided. 
-
-    Example
-    -------
-    getForecastData(country = 'United States', indicator = 'Imports')
-
-    getForecastData(country = ['United States', 'India'], indicator = ['Imports','Exports'])
-    """
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-
-    if country == None and indicator == None:
-        raise ValueError ('At least one of the parameters, country or indicator, needs to be supplied.')
-    elif country != None and indicator == None:
-        linkAPI = checkCountry(country)
-    elif country == None and indicator != None:
-        linkAPI = checkIndic(indicator)
-    else:
-        linkAPI = getLink(country, indicator)
-    try:
-        linkAPI += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-    try:
-        #print(linkAPI)
-        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
-    except Exception as e:
-        print(e)
-       
-
-
-def getForecastByTicker(ticker=None, output_type=None):
-    """
-    Returns a list of Forecast by specific ticker.
-    =================================================================================
-    Parameters:
-    -----------
-        ticker: string or list.
-                ticker = 'USURTOT'
-                ticker = ['WGDPCHIN', 'USURTOT']    
-        output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web. 
-    Notes
-    -----
-     
-    
-    Example
-    -------
-            getForecastByTicker(ticker = 'USURTOT', output_type = 'df')
-
-            getForecastByTicker(ticker = ['WGDPCHIN', 'USURTOT'], output_type = 'df')
-    """
-    
-    # d is a dictionary used for create the api url
-    d = {
-        'url_base': 'https://api.tradingeconomics.com/forecast',
-        'country': '',
-        'ticker' : '',
-        'key': f'?c={glob.apikey}',
-        'output_type' : ''
-    }
-
-    if ticker:
-        d['ticker']=f'/ticker/{fn.stringOrList(ticker)}'
-        api_url_request = "%s%s%s" % (d['url_base'], d['ticker'],  d['key']) 
-        # print(api_url_request)
-        return fn.dataRequest(api_request=api_url_request, output_type=output_type)
-        
-         
-
-    return 'Ticker is required'
-        
-
+import json 
+import urllib 
+import pandas as pd
+from datetime import *
+import sys
+from . import functions as fn
+from . import glob
+import ssl
+
+PY3 = sys.version_info[0] == 3
+
+if PY3: # Python 3+
+    from urllib.request import urlopen
+    from urllib.parse import quote
+else: # Python 2.X
+    from urllib import urlopen
+    from urllib import quote
+      
+
+class ParametersError(ValueError):
+    pass
+
+class CredentialsError(ValueError):
+    pass
+
+class LoginError(AttributeError):
+    pass
+  
+class WebRequestError(ValueError):
+    pass
+  
+def checkCountry(country):
+    linkAPI = 'https://api.tradingeconomics.com/forecast/country/'       
+    if type(country) is str:
+        linkAPI += quote(country, safe='')
+    else:
+        #multiCountry = ",".join(country)
+        linkAPI += quote(",".join(country), safe='')
+    return linkAPI
+        
+def checkIndic(indicator):
+    linkAPI = 'https://api.tradingeconomics.com/forecast/indicator/'        
+    if type(indicator) is str:
+        linkAPI += quote(indicator, safe='')
+    else:
+        #multiIndic = ",".join(indicator)
+        linkAPI += quote(",".join(indicator), safe='')
+    return linkAPI
+
+def getLink(country, indicator):
+    linkAPI = 'https://api.tradingeconomics.com/forecast/country/'
+    if type(country) is str:
+        linkAPI += quote(country)
+    else:
+        #multiCountry = ",".join(country)
+        linkAPI += quote(",".join(country), safe='') 
+    if type(indicator) is str:
+        linkAPI += '/indicator/' + quote(indicator, safe='')
+    else:
+        #multiIndic = ",".join(indicator)
+        linkAPI += '/indicator/' + quote(",".join(indicator), safe='') 
+    return linkAPI
+
+    
+def getForecastData(country = None, indicator = None, output_type = None):
+    """
+     Return forecast values by country, by indicator, by country and indicator.
+    ===========================================================================
+
+    Parameters:
+    -----------
+    country: string or list.
+             String to get data for one country. List of strings to get data for
+             several countries. For example, country = ['United States', 'Australia'].
+    indicator: string or list.
+             String  to get data for one category. List of strings to get data for several calendar events.
+             For example, category = 'GDP Growth Rate' or 
+             category = ['Exports', 'Imports']
+    output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries without any parsing.  
+
+    Notes
+    -----
+    At least one of parameters, country or indicator, should be provided. 
+
+    Example
+    -------
+    getForecastData(country = 'United States', indicator = 'Imports')
+
+    getForecastData(country = ['United States', 'India'], indicator = ['Imports','Exports'])
+    """
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+
+    if country == None and indicator == None:
+        raise ValueError ('At least one of the parameters, country or indicator, needs to be supplied.')
+    elif country != None and indicator == None:
+        linkAPI = checkCountry(country)
+    elif country == None and indicator != None:
+        linkAPI = checkIndic(indicator)
+    else:
+        linkAPI = getLink(country, indicator)
+    try:
+        linkAPI += '?c=' + glob.apikey
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+    try:
+        #print(linkAPI)
+        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
+    except Exception as e:
+        print(e)
+       
+
+
+def getForecastByTicker(ticker=None, output_type=None):
+    """
+    Returns a list of Forecast by specific ticker.
+    =================================================================================
+    Parameters:
+    -----------
+        ticker: string or list.
+                ticker = 'USURTOT'
+                ticker = ['WGDPCHIN', 'USURTOT']    
+        output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+    Notes
+    -----
+     
+    
+    Example
+    -------
+            getForecastByTicker(ticker = 'USURTOT', output_type = 'df')
+
+            getForecastByTicker(ticker = ['WGDPCHIN', 'USURTOT'], output_type = 'df')
+    """
+    
+    # d is a dictionary used for create the api url
+    d = {
+        'url_base': 'https://api.tradingeconomics.com/forecast',
+        'country': '',
+        'ticker' : '',
+        'key': f'?c={glob.apikey}',
+        'output_type' : ''
+    }
+
+    if ticker:
+        d['ticker']=f'/ticker/{fn.stringOrList(ticker)}'
+        api_url_request = "%s%s%s" % (d['url_base'], d['ticker'],  d['key']) 
+        # print(api_url_request)
+        return fn.dataRequest(api_request=api_url_request, output_type=output_type)
+        
+         
+
+    return 'Ticker is required'
+        
+
```

### Comparing `tradingeconomics-4.2.8/tradingeconomics/functions.py` & `tradingeconomics-4.2.9/tradingeconomics/functions.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,243 +1,243 @@
-
-from datetime import *
-import re
-import itertools
-import urllib
-import sys
-import json
-import pandas as pd
-import time
-
-PY3 = sys.version_info[0] == 3
-
-if PY3: # Python 3+
-    from urllib.request import urlopen
-    from urllib.parse import quote
-else: # Python 2.X
-    from urllib import urlopen
-    from urllib import quote
-
-
-class DateError(ValueError):
-    pass
-
-class CredentialsError(ValueError):
-    pass
-
-def credCheck(credentials):
-    #pattern = re.compile("^:$")
-    #if not(pattern.match(credentials)):
-    #    raise CredentialsError('Invalid credentials.')
-    if ':' not in credentials:
-        raise CredentialsError('Invalid credentials.')
-    
-
-def out_type(init_format, isCommodity = False):
-    if isCommodity:
-        list_of_countries= init_format.Title.unique()
-    else:
-        list_of_countries= init_format.Country.unique()
-    list_of_cat= init_format.Category.unique()
-    dict_start = {el:{elm:0 for elm in list_of_cat} for el in list_of_countries} 
-    for i, j in itertools.product(range(len(list_of_countries)), range(len(list_of_cat))):
-        if isCommodity:
-            dict_cntry = init_format.loc[init_format['Title'] == list_of_countries[i]]
-        else:
-            dict_cntry = init_format.loc[init_format['Country'] == list_of_countries[i]]
-        dict_cat = dict_cntry.loc[init_format['Category'] == list_of_cat[j]].to_dict('records')
-        dict_start[list_of_countries[i]][list_of_cat[j]] = dict_cat
-        for l in range(len(dict_cat)):
-            if isCommodity:
-                del dict_cat[l]['Title']
-            else:
-                del dict_cat[l]['Country']
-            del dict_cat[l]['Category']
-    return dict_start
-       
-       
-def validate(date_text):      
-        try:
-            try:
-                datetime.strptime(date_text, '%Y-%m-%d')
-            except:
-                datetime.strptime(date_text, '%Y-%m-%d %H:%M')
-        except ValueError:
-            raise DateError("Incorrect data format, should be YYYY-MM-DD")
-                       
-def validatePeriod(initDate, endDate):
-    if  datetime.strptime(initDate, '%Y-%m-%d') > datetime.strptime(endDate, '%Y-%m-%d'):
-        raise DateError ('Invalid time period, check the supplied date parameters.')
-
-def timeValidate(clientTime):
-    try:
-        t = time.strptime(clientTime, '%H:%M')
-        time.strftime('%H:%M', t)
-    except ValueError:
-        print("Incorrect time format, should be HH:MM")
-
-def finalLink(link, prmtr):
-    linkAPI  = link
-    for i in range(len(prmtr)):
-        if type(prmtr) == str: 
-            linkAPI = linkAPI + '/' + prmtr
-        linkAPI = linkAPI + '/' + str( prmtr[i])            
-    return linkAPI
-
-def stringOrList(string_or_list):
-    if type(string_or_list) is not str:
-        return quote(",".join(string_or_list))
-    return quote(string_or_list)
-
-def stringOrListWithAppend(string_or_list_1, string_or_list_2):
-    if type(string_or_list_1) is list:
-        _list_1 = [s for s in string_or_list_1]
-    elif type(string_or_list_1) is str:
-        _list_1 = [string_or_list_1]
-    
-    if type(string_or_list_2) is list:
-        _list_2 = [s for s in string_or_list_2]
-    elif type(string_or_list_2) is str:
-        _list_2 = [string_or_list_2]
-
-    combinations = list(itertools.product(_list_1,_list_2))
-    comb = [':'.join(c) for c in combinations]
-    return quote(f','.join(comb))
-
-def dataRequest(api_request, output_type):
-    def trimTheResponse(webResultsRaw):
-            finalResultsList = []
-            while len(webResultsRaw)>0:
-                oneDict = {}
-                oneItem = webResultsRaw.pop()
-                oneItemTrimedArray = list(map(lambda x: [x[0],x[1].rstrip()] if (str(type(x[1])) == "<class 'str'>") else [x[0], x[1]] ,list(oneItem.items())))
-                while len(oneItemTrimedArray)>0:
-                    oneTrimmedItem = oneItemTrimedArray.pop(0)
-                    oneDict[oneTrimmedItem[0]] = oneTrimmedItem[1]
-                finalResultsList.append(oneDict)
-            return finalResultsList
-    def outputTypeCheck(outputType):
-        if outputType not in (None, 'raw', 'dict','df'):
-            raise ParametersError ('invalid output_type')
-    class ParametersError(ValueError):
-        pass
-    
-
-    class WebRequestError(ValueError):
-        pass
-
-
-    outputTypeCheck(output_type)
-    
-    try:
-        response = urlopen(api_request)
-        code = response.getcode()
-        webResultsRaw = json.loads(response.read().decode('utf-8'))
-        webResults = trimTheResponse(webResultsRaw)
-    except ValueError:
-        if code != 200:
-            print(urlopen(api_request).read().decode('utf-8'))
-        else: 
-            raise WebRequestError ('Something went wrong. Error code = ' + str(code))
-    if code == 200:
-        try:
-            
-            if len(webResults) > 0:
-                #names = ['country', 'category', 'historicalDataSymbol', 'lastUpdate']
-                #names2 = ['Country', 'Category', 'HistoricalDataSymbol', 'LastUpdate']   
-                maindf = pd.DataFrame(webResults)#columns=names2    
-            
-            else:
-                raise ParametersError ('No data available for the provided parameters.')
-            if output_type == None or output_type =='dict':
-                output = webResults
-                # output = maindf.to_dict('dict')
-            elif output_type == 'df':        
-                output = maindf
-            elif output_type == 'raw':        
-                output = webResults
-            else:      
-                raise ParametersError ('output_type options : df(default) for data frame or raw for unparsed results.') 
-            return output
-        except ValueError:
-            pass
-    else:
-        return ''    
-
-def makeRequestAndParse(api_request, output_type):
-    class ParametersError(ValueError):
-        pass
-
-    class WebRequestError(ValueError):
-        pass
-
-
-    try:
-        response = urlopen(api_request)
-        code = response.getcode()
-        webResults = json.loads(response.read().decode('utf-8'))
-    except ValueError:
-        if code != 200:
-            print(urlopen(api_request).read().decode('utf-8'))
-        else: 
-            raise WebRequestError ('Something went wrong. Error code = ' + str(code))
-    if code == 200:
-        try:
-            
-            if len(webResults) > 0:
-                #names = ['country', 'category', 'historicalDataSymbol', 'lastUpdate']
-                #names2 = ['Country', 'Category', 'HistoricalDataSymbol', 'LastUpdate']   
-                maindf = pd.DataFrame.from_records(webResults)#columns=names2    
-            
-            else:
-                raise ParametersError ('No data available for the provided parameters.')
-            if output_type == None or output_type =='dict':
-                output = maindf.to_dict('dict')
-            elif output_type == 'df':        
-                output = maindf
-            elif output_type == 'raw':        
-                output = webResults
-            else:      
-                raise ParametersError ('output_type options : df(default) for data frame or raw for unparsed results.') 
-            return output
-        except ValueError:
-            pass
-    else:
-        return ''   
-
-def checkDates(baseLink, initDate=None, endDate=None):
-    if (initDate is not None) and endDate == None :
-        try: 
-            validate(initDate)
-        except ValueError:
-            raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
-        # if initDate > str(date.today()):
-        #     raise DateError ('Initial date out of range.')
-        baseLink += '&d1=' + quote(initDate)
-
-    if (initDate is not None) and (endDate is not None) :
-        try: 
-            validate(initDate)
-        except ValueError:
-            raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
-        try: 
-            validate(endDate)
-        except ValueError:
-            raise DateError ('Incorrect endDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
-        try:        
-            validatePeriod(initDate, endDate)
-        except ValueError:
-            raise DateError ('Invalid time period.')
-        baseLink += '&d1=' + quote(initDate) + '&d2=' + quote(endDate)
-
-    if initDate == None and (endDate is not None):
-        raise DateError('initDate value is missing')
-    return baseLink
-
-
-def isStringOrList(string_or_list):
-    if type(string_or_list) is str:
-        return quote(string_or_list)
-    elif type(string_or_list) is list:
-        return quote(",".join(string_or_list))
-    else:
-        raise ValueError('Invalid input type. Should be string or list of strings.')
+
+from datetime import *
+import re
+import itertools
+import urllib
+import sys
+import json
+import pandas as pd
+import time
+
+PY3 = sys.version_info[0] == 3
+
+if PY3: # Python 3+
+    from urllib.request import urlopen
+    from urllib.parse import quote
+else: # Python 2.X
+    from urllib import urlopen
+    from urllib import quote
+
+
+class DateError(ValueError):
+    pass
+
+class CredentialsError(ValueError):
+    pass
+
+def credCheck(credentials):
+    #pattern = re.compile("^:$")
+    #if not(pattern.match(credentials)):
+    #    raise CredentialsError('Invalid credentials.')
+    if ':' not in credentials:
+        raise CredentialsError('Invalid credentials.')
+    
+
+def out_type(init_format, isCommodity = False):
+    if isCommodity:
+        list_of_countries= init_format.Title.unique()
+    else:
+        list_of_countries= init_format.Country.unique()
+    list_of_cat= init_format.Category.unique()
+    dict_start = {el:{elm:0 for elm in list_of_cat} for el in list_of_countries} 
+    for i, j in itertools.product(range(len(list_of_countries)), range(len(list_of_cat))):
+        if isCommodity:
+            dict_cntry = init_format.loc[init_format['Title'] == list_of_countries[i]]
+        else:
+            dict_cntry = init_format.loc[init_format['Country'] == list_of_countries[i]]
+        dict_cat = dict_cntry.loc[init_format['Category'] == list_of_cat[j]].to_dict('records')
+        dict_start[list_of_countries[i]][list_of_cat[j]] = dict_cat
+        for l in range(len(dict_cat)):
+            if isCommodity:
+                del dict_cat[l]['Title']
+            else:
+                del dict_cat[l]['Country']
+            del dict_cat[l]['Category']
+    return dict_start
+       
+       
+def validate(date_text):      
+        try:
+            try:
+                datetime.strptime(date_text, '%Y-%m-%d')
+            except:
+                datetime.strptime(date_text, '%Y-%m-%d %H:%M')
+        except ValueError:
+            raise DateError("Incorrect data format, should be YYYY-MM-DD")
+                       
+def validatePeriod(initDate, endDate):
+    if  datetime.strptime(initDate, '%Y-%m-%d') > datetime.strptime(endDate, '%Y-%m-%d'):
+        raise DateError ('Invalid time period, check the supplied date parameters.')
+
+def timeValidate(clientTime):
+    try:
+        t = time.strptime(clientTime, '%H:%M')
+        time.strftime('%H:%M', t)
+    except ValueError:
+        print("Incorrect time format, should be HH:MM")
+
+def finalLink(link, prmtr):
+    linkAPI  = link
+    for i in range(len(prmtr)):
+        if type(prmtr) == str: 
+            linkAPI = linkAPI + '/' + prmtr
+        linkAPI = linkAPI + '/' + str( prmtr[i])            
+    return linkAPI
+
+def stringOrList(string_or_list):
+    if type(string_or_list) is not str:
+        return quote(",".join(string_or_list))
+    return quote(string_or_list)
+
+def stringOrListWithAppend(string_or_list_1, string_or_list_2):
+    if type(string_or_list_1) is list:
+        _list_1 = [s for s in string_or_list_1]
+    elif type(string_or_list_1) is str:
+        _list_1 = [string_or_list_1]
+    
+    if type(string_or_list_2) is list:
+        _list_2 = [s for s in string_or_list_2]
+    elif type(string_or_list_2) is str:
+        _list_2 = [string_or_list_2]
+
+    combinations = list(itertools.product(_list_1,_list_2))
+    comb = [':'.join(c) for c in combinations]
+    return quote(f','.join(comb))
+
+def dataRequest(api_request, output_type):
+    def trimTheResponse(webResultsRaw):
+            finalResultsList = []
+            while len(webResultsRaw)>0:
+                oneDict = {}
+                oneItem = webResultsRaw.pop()
+                oneItemTrimedArray = list(map(lambda x: [x[0],x[1].rstrip()] if (str(type(x[1])) == "<class 'str'>") else [x[0], x[1]] ,list(oneItem.items())))
+                while len(oneItemTrimedArray)>0:
+                    oneTrimmedItem = oneItemTrimedArray.pop(0)
+                    oneDict[oneTrimmedItem[0]] = oneTrimmedItem[1]
+                finalResultsList.append(oneDict)
+            return finalResultsList
+    def outputTypeCheck(outputType):
+        if outputType not in (None, 'raw', 'dict','df'):
+            raise ParametersError ('invalid output_type')
+    class ParametersError(ValueError):
+        pass
+    
+
+    class WebRequestError(ValueError):
+        pass
+
+
+    outputTypeCheck(output_type)
+    
+    try:
+        response = urlopen(api_request)
+        code = response.getcode()
+        webResultsRaw = json.loads(response.read().decode('utf-8'))
+        webResults = trimTheResponse(webResultsRaw)
+    except ValueError:
+        if code != 200:
+            print(urlopen(api_request).read().decode('utf-8'))
+        else: 
+            raise WebRequestError ('Something went wrong. Error code = ' + str(code))
+    if code == 200:
+        try:
+            
+            if len(webResults) > 0:
+                #names = ['country', 'category', 'historicalDataSymbol', 'lastUpdate']
+                #names2 = ['Country', 'Category', 'HistoricalDataSymbol', 'LastUpdate']   
+                maindf = pd.DataFrame(webResults)#columns=names2    
+            
+            else:
+                raise ParametersError ('No data available for the provided parameters.')
+            if output_type == None or output_type =='dict':
+                output = webResults
+                # output = maindf.to_dict('dict')
+            elif output_type == 'df':        
+                output = maindf
+            elif output_type == 'raw':        
+                output = webResults
+            else:      
+                raise ParametersError ('output_type options : df(default) for data frame or raw for unparsed results.') 
+            return output
+        except ValueError:
+            pass
+    else:
+        return ''    
+
+def makeRequestAndParse(api_request, output_type):
+    class ParametersError(ValueError):
+        pass
+
+    class WebRequestError(ValueError):
+        pass
+
+
+    try:
+        response = urlopen(api_request)
+        code = response.getcode()
+        webResults = json.loads(response.read().decode('utf-8'))
+    except ValueError:
+        if code != 200:
+            print(urlopen(api_request).read().decode('utf-8'))
+        else: 
+            raise WebRequestError ('Something went wrong. Error code = ' + str(code))
+    if code == 200:
+        try:
+            
+            if len(webResults) > 0:
+                #names = ['country', 'category', 'historicalDataSymbol', 'lastUpdate']
+                #names2 = ['Country', 'Category', 'HistoricalDataSymbol', 'LastUpdate']   
+                maindf = pd.DataFrame.from_records(webResults)#columns=names2    
+            
+            else:
+                raise ParametersError ('No data available for the provided parameters.')
+            if output_type == None or output_type =='dict':
+                output = maindf.to_dict('dict')
+            elif output_type == 'df':        
+                output = maindf
+            elif output_type == 'raw':        
+                output = webResults
+            else:      
+                raise ParametersError ('output_type options : df(default) for data frame or raw for unparsed results.') 
+            return output
+        except ValueError:
+            pass
+    else:
+        return ''   
+
+def checkDates(baseLink, initDate=None, endDate=None):
+    if (initDate is not None) and endDate == None :
+        try: 
+            validate(initDate)
+        except ValueError:
+            raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
+        # if initDate > str(date.today()):
+        #     raise DateError ('Initial date out of range.')
+        baseLink += '&d1=' + quote(initDate)
+
+    if (initDate is not None) and (endDate is not None) :
+        try: 
+            validate(initDate)
+        except ValueError:
+            raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
+        try: 
+            validate(endDate)
+        except ValueError:
+            raise DateError ('Incorrect endDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
+        try:        
+            validatePeriod(initDate, endDate)
+        except ValueError:
+            raise DateError ('Invalid time period.')
+        baseLink += '&d1=' + quote(initDate) + '&d2=' + quote(endDate)
+
+    if initDate == None and (endDate is not None):
+        raise DateError('initDate value is missing')
+    return baseLink
+
+
+def isStringOrList(string_or_list):
+    if type(string_or_list) is str:
+        return quote(string_or_list)
+    elif type(string_or_list) is list:
+        return quote(",".join(string_or_list))
+    else:
+        raise ValueError('Invalid input type. Should be string or list of strings.')
```

### Comparing `tradingeconomics-4.2.8/tradingeconomics/historical.py` & `tradingeconomics-4.2.9/tradingeconomics/historical.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,350 +1,350 @@
-import json
-import itertools
-import urllib 
-import pandas as pd
-import sys
-from datetime import *
-from dateutil.relativedelta import relativedelta
-from . import functions as fn
-from . import glob
-import ssl
-
-PY3 = sys.version_info[0] == 3
-
-if PY3: # Python 3+
-    from urllib.request import urlopen
-    from urllib.parse import quote
-else: # Python 2.X
-    from urllib import urlopen
-    from urllib import quote
-
-class ParametersError(ValueError):
-    pass
-
-class DateError(ValueError):
-    pass
-
-class CredentialsError(ValueError):
-    pass
-
-class LoginError(AttributeError):
-    pass
-
-class WebRequestError(ValueError):
-    pass
-
-def parseData(data):
-        indx = pd.DatetimeIndex(data['dates'])
-        datafr = pd.DataFrame(data['values']) 
-        datafr = datafr.set_index(indx)
-        return datafr    
-        
-def multiParams(webdata):
-    mycntry = list(set([d['Country'] for d in webdata]))
-    myind = list(set([d['Category'] for d in webdata]))
-    lst = [(d['Country'], d['Value'], d['DateTime'], d['Category']) for d in webdata] 
-    lst2 = [list(i) for i in lst]
-    countryDict = dict();
-    for i in range(len(mycntry)):
-        countryDict[mycntry[i]] = dict();
-        for m in range(len(myind)):
-            countryDict[mycntry[i]][myind[m]] = {'dates':list(), 'values': list()}
-            for j in range(len(lst2)):                
-                if lst2[j][0] == mycntry[i] and lst2[j][3] == myind[m]:
-                    countryDict[mycntry[i]][myind[m]]['dates'].append(lst2[j][2])
-                    countryDict[mycntry[i]][myind[m]]['values'].append(lst2[j][1])
-    finalDict = multiParsedData(countryDict)                            
-    return finalDict 
-          
-def multiParsedData(countryDict):
-    CNTRY = list(countryDict.keys())
-    INDCTR = list(countryDict[CNTRY[0]].keys())
-    answer = [];
-    for i, j in itertools.product(range(len(CNTRY)), range(len(INDCTR))):
-        answer.append(parseData(countryDict[CNTRY[i]][INDCTR[j]]).to_dict('Series').values())
-    empty_dict2 =  dict.fromkeys(CNTRY)
-    for i in range(len(CNTRY)):
-        empty_dict2[CNTRY[i]] = dict.fromkeys(INDCTR)    
-    for i, j in itertools.product(range(len(CNTRY)), range(len(INDCTR))):
-        empty_dict2[CNTRY[i]][INDCTR[j]] = answer[:1]
-        del answer[0]       
-    return empty_dict2      
-
-def out_type(init_format):
-    list_of_countries= init_format.Country.unique()
-    list_of_cat= init_format.Category.unique()
-    dict_start = {el:{elm:0 for elm in list_of_cat} for el in list_of_countries} 
-    for i, j in itertools.product(range(len(list_of_countries)), range(len(list_of_cat))):
-        dict_cntry = init_format.loc[init_format['Country'] == list_of_countries[i]]
-        dict_cat = dict_cntry.loc[init_format['Category'] == list_of_cat[j]].to_dict('records')
-        dict_start[list_of_countries[i]][list_of_cat[j]] = dict_cat
-        for l in range(len(dict_cat)):
-            del dict_cat[l]['Country']
-            del dict_cat[l]['Category']
-    return dict_start
-            
-def paramCheck (country, indicator):
-    linkAPI = 'https://api.tradingeconomics.com/historical/country/'
-    if type(country) is str:
-        linkAPI += quote(country)
-    else:
-        linkAPI += quote(",".join(country), safe='') 
-    if type(indicator) is str:
-        linkAPI += '/indicator/' + quote(indicator, safe='')
-    else:
-        linkAPI += '/indicator/' + quote(",".join(indicator), safe='') 
-    return linkAPI
-
-def checkCountryHistoricalRatings(country):
-    linkAPI = 'https://api.tradingeconomics.com/ratings/historical/'       
-    if type(country) is str:
-        linkAPI += quote(country.lower())
-    else:
-        linkAPI += quote(",".join(country), safe='')
-    return linkAPI
-    
-def getRatingResults(webResults, rating):
-        names = ['country','date', 'agency', 'rating', 'outlook']
-        names2 = ['Country','Date', 'Agency', 'Rating', 'Outlook']
-        maindf = pd.DataFrame()  
-        for i in range(len(names)):  
-            names[i] = [d[names2[i]]  for d in webResults]
-            maindf = pd.concat([maindf, pd.DataFrame(names[i], columns = [names2[i]])], axis = 1) 
-        maindf['Rating'] =  maindf['Rating'].map(lambda x: x.strip())
-        return maindf
-
-def checkRatings(linkAPI, rating):    
-    if type(rating) is str:
-        linkAPI += 'https://api.tradingeconomics.com/ratings/historical/' + quote(rating)
-    else:
-        linkAPI += 'https://api.tradingeconomics.com/ratings/historical/' + quote(",".join(rating))
-    return linkAPI    
-
-
-def getHistoricalData(country = None, indicator = None, initDate= None, endDate= None, output_type = None):
-    """
-    Return historical information for specific country and indicator.
-    =================================================================
-    Parameters:
-    -----------
-    country: string or list.
-             String to get data for one country. List of strings to get data for
-             several countries. For example, country = ['United States', 'Australia'].
-    indicator: string or list.
-             String  to get data for one category. List of strings to get data for several calendar events.
-             For example, category = 'GDP Growth Rate' or 
-             category = ['Exports', 'Imports']
-    initDate: string with format: YYYY-MM-DD.
-             For example: '2011-01-01' 
-    endDate: string with format: YYYY-MM-DD.
-    output_type: string.
-             'dict'(default) for dictionary format output,
-             'raw' for list of dictionaries without any parsing.
-    Notes
-    ----- 
-    Must choose a country and an indicator.
-    Example
-    -------
-    getHistoricalData(country = 'United States', indicator = 'Imports', initDate = '2011-01-01', endDate = '2016-01-01')
-    getHistoricalData(country = ['United States', 'china'], indicator = ['Imports','Exports'], initDate = '2011-01-01', endDate = '2016-01-01')
-    """
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-
-    if type(country) is str and type(indicator) is str: 
-        linkAPI = 'https://api.tradingeconomics.com/historical/country/' + quote(country)  + '/indicator/' + quote(indicator) 
-    else:
-        linkAPI = paramCheck(country, indicator)
-        
-    if initDate == None and endDate == None:
-        minDate = [(datetime.now() - relativedelta(years=15)).strftime('%Y-%m-%d') ]
-        linkAPI = fn.finalLink(linkAPI, minDate) 
-    if initDate == None and (endDate is not None): 
-        raise DateError('initDate value is missing') 
-    if (initDate is not None) and (endDate is not None) :
-        try: 
-            fn.validate(initDate)
-        except ValueError:
-            raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
-        try: 
-            fn.validate(endDate)
-        except ValueError:
-            raise DateError ('Incorrect endDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
-        try:        
-            fn.validatePeriod(initDate, endDate)
-        except ValueError:
-            raise DateError ('Invalid time period.')
-        linkAPI = fn.finalLink(linkAPI, [initDate, endDate])
-    if (initDate is not None) and endDate == None :        
-        try: 
-            fn.validate(initDate)
-        except ValueError:
-            raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
-            if initDate > str(date.today()):
-                raise DateError ('Initial date out of range.')
-        linkAPI = fn.finalLink(linkAPI, [initDate])
-   
-    try:
-        linkAPI += '?c='+glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-    
-    try:
-        #print(linkAPI)
-        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
-    except Exception as e:
-        print(e)  
-        
-
-def getHistoricalRatings(country = None, rating = None, initDate = None, endDate=None, output_type = None):
-    """
-    Return historical information for specific country.
-    =================================================================
-    Parameters:
-    -----------
-    country: string or list.
-             String to get data for one country. List of strings to get data for
-             several countries. For example, country = ['United States', 'Australia'].
-        output_type: string.
-             'df'(default) for dictionary format output,
-             'raw' for list of dictionaries without any parsing.
-    Notes
-    ----- 
-    Without credentials only sample data will be provided.
-    Example
-    -------
-    getHistoricalRatings(country = 'United States', rating = None)
-    getHistoricalRatings(country = ['United States', 'United Kingdom'], rating = None)
-    getHistoricalRatings(country = 'United States', initDate ='2011-01-01')
-    getHistoricalRatings(country = 'United States', initDate ='2011-01-01', endDate = '2012-01-01')
-    
-    """
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-    
-    if country == None:
-        linkAPI = 'https://api.tradingeconomics.com/ratings/historical/'    
-    else:
-         linkAPI = checkCountryHistoricalRatings(country)
-        
-    if rating == None:
-        linkAPI = linkAPI
-    else:
-        linkAPI = checkRatings(linkAPI, rating)
-    if (country == None) and (rating == None):
-        linkAPI = 'https://api.tradingeconomics.com/ratings/historical/united%20states'   
-    else:
-        linkAPI = linkAPI
-    if (initDate is not None) and (endDate == None):
-        linkAPI = checkCountryHistoricalRatings(country) + "/" + initDate
-    elif (initDate is not None) and (endDate is not None):
-        linkAPI = checkCountryHistoricalRatings(country) + "/" + initDate + "/" + endDate
-    try:
-        linkAPI += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-   
-    try:
-        #print(linkAPI)
-        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
-    except Exception as e:
-        print(e)   
-
-def getHistoricalByTicker(ticker=None, start_date=None, output_type=None):
-    """
-    Returns historical data by ticker.
-    =================================================================================
-    Parameters:
-    -----------
-        ticker: string.
-                ticker = 'USURTOT'
-        start_date: string.
-                start_date = '2015-03-01
-        output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web. 
-    Notes
-    -----
-    start_date is optional 
-    
-    Example
-    -------
-            getIndicatorByTicker(ticker = 'USURTOT', output_type = 'df')
-
-            getIndicatorByTicker(ticker = 'USURTOT', start_date = '2015-03-01, output_type = 'df')
-    """
-    
-    # d is a dictionary used for create the api url
-    d = {
-        'url_base': 'https://api.tradingeconomics.com/historical',
-        'country': '',
-        'ticker' : '',
-        'start_date': '',
-        'key': f'?c={glob.apikey}',
-        'output_type' : ''
-    }
-    if start_date :        
-        try: 
-            fn.validate(start_date)
-        except ValueError:
-            raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
-            
-
-    if ticker:
-        d['ticker']=f'/ticker/{fn.stringOrList(ticker)}'
-        d['start_date']=f'/{start_date}'
-        api_url_request = "%s%s%s%s" % (d['url_base'], d['ticker'],  d['start_date'],  d['key']) 
-        #print(api_url_request)
-        return fn.dataRequest(api_request=api_url_request, output_type=output_type)
-        #return
-         
-
-    return 'Ticker is required'
-
-
-def getHistoricalUpdates(output_type=None):
-    """
-    Returns historical Update.
-    =================================================================================
-    Parameters:
-    -----------
-        
-        output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web. 
-    Notes
-    -----
-    
-    
-    Example
-    -------
-            getHistoricalUpdates(output_type = 'df')
-
-
-    """
-    
-    # d is a dictionary used for create the api url
-    d = {
-        'url_base': 'https://api.tradingeconomics.com/historical/updates',
-        'key': f'?c={glob.apikey}',
-        'output_type' : ''
-    }
-    
-    api_url_request = "%s%s" % (d['url_base'], d['key']) 
-    #print(api_url_request)
-    return fn.dataRequest(api_request=api_url_request, output_type=output_type)
-
-    
-    
-         
-
-    
-    
+import json
+import itertools
+import urllib 
+import pandas as pd
+import sys
+from datetime import *
+from dateutil.relativedelta import relativedelta
+from . import functions as fn
+from . import glob
+import ssl
+
+PY3 = sys.version_info[0] == 3
+
+if PY3: # Python 3+
+    from urllib.request import urlopen
+    from urllib.parse import quote
+else: # Python 2.X
+    from urllib import urlopen
+    from urllib import quote
+
+class ParametersError(ValueError):
+    pass
+
+class DateError(ValueError):
+    pass
+
+class CredentialsError(ValueError):
+    pass
+
+class LoginError(AttributeError):
+    pass
+
+class WebRequestError(ValueError):
+    pass
+
+def parseData(data):
+        indx = pd.DatetimeIndex(data['dates'])
+        datafr = pd.DataFrame(data['values']) 
+        datafr = datafr.set_index(indx)
+        return datafr    
+        
+def multiParams(webdata):
+    mycntry = list(set([d['Country'] for d in webdata]))
+    myind = list(set([d['Category'] for d in webdata]))
+    lst = [(d['Country'], d['Value'], d['DateTime'], d['Category']) for d in webdata] 
+    lst2 = [list(i) for i in lst]
+    countryDict = dict();
+    for i in range(len(mycntry)):
+        countryDict[mycntry[i]] = dict();
+        for m in range(len(myind)):
+            countryDict[mycntry[i]][myind[m]] = {'dates':list(), 'values': list()}
+            for j in range(len(lst2)):                
+                if lst2[j][0] == mycntry[i] and lst2[j][3] == myind[m]:
+                    countryDict[mycntry[i]][myind[m]]['dates'].append(lst2[j][2])
+                    countryDict[mycntry[i]][myind[m]]['values'].append(lst2[j][1])
+    finalDict = multiParsedData(countryDict)                            
+    return finalDict 
+          
+def multiParsedData(countryDict):
+    CNTRY = list(countryDict.keys())
+    INDCTR = list(countryDict[CNTRY[0]].keys())
+    answer = [];
+    for i, j in itertools.product(range(len(CNTRY)), range(len(INDCTR))):
+        answer.append(parseData(countryDict[CNTRY[i]][INDCTR[j]]).to_dict('Series').values())
+    empty_dict2 =  dict.fromkeys(CNTRY)
+    for i in range(len(CNTRY)):
+        empty_dict2[CNTRY[i]] = dict.fromkeys(INDCTR)    
+    for i, j in itertools.product(range(len(CNTRY)), range(len(INDCTR))):
+        empty_dict2[CNTRY[i]][INDCTR[j]] = answer[:1]
+        del answer[0]       
+    return empty_dict2      
+
+def out_type(init_format):
+    list_of_countries= init_format.Country.unique()
+    list_of_cat= init_format.Category.unique()
+    dict_start = {el:{elm:0 for elm in list_of_cat} for el in list_of_countries} 
+    for i, j in itertools.product(range(len(list_of_countries)), range(len(list_of_cat))):
+        dict_cntry = init_format.loc[init_format['Country'] == list_of_countries[i]]
+        dict_cat = dict_cntry.loc[init_format['Category'] == list_of_cat[j]].to_dict('records')
+        dict_start[list_of_countries[i]][list_of_cat[j]] = dict_cat
+        for l in range(len(dict_cat)):
+            del dict_cat[l]['Country']
+            del dict_cat[l]['Category']
+    return dict_start
+            
+def paramCheck (country, indicator):
+    linkAPI = 'https://api.tradingeconomics.com/historical/country/'
+    if type(country) is str:
+        linkAPI += quote(country)
+    else:
+        linkAPI += quote(",".join(country), safe='') 
+    if type(indicator) is str:
+        linkAPI += '/indicator/' + quote(indicator, safe='')
+    else:
+        linkAPI += '/indicator/' + quote(",".join(indicator), safe='') 
+    return linkAPI
+
+def checkCountryHistoricalRatings(country):
+    linkAPI = 'https://api.tradingeconomics.com/ratings/historical/'       
+    if type(country) is str:
+        linkAPI += quote(country.lower())
+    else:
+        linkAPI += quote(",".join(country), safe='')
+    return linkAPI
+    
+def getRatingResults(webResults, rating):
+        names = ['country','date', 'agency', 'rating', 'outlook']
+        names2 = ['Country','Date', 'Agency', 'Rating', 'Outlook']
+        maindf = pd.DataFrame()  
+        for i in range(len(names)):  
+            names[i] = [d[names2[i]]  for d in webResults]
+            maindf = pd.concat([maindf, pd.DataFrame(names[i], columns = [names2[i]])], axis = 1) 
+        maindf['Rating'] =  maindf['Rating'].map(lambda x: x.strip())
+        return maindf
+
+def checkRatings(linkAPI, rating):    
+    if type(rating) is str:
+        linkAPI += 'https://api.tradingeconomics.com/ratings/historical/' + quote(rating)
+    else:
+        linkAPI += 'https://api.tradingeconomics.com/ratings/historical/' + quote(",".join(rating))
+    return linkAPI    
+
+
+def getHistoricalData(country = None, indicator = None, initDate= None, endDate= None, output_type = None):
+    """
+    Return historical information for specific country and indicator.
+    =================================================================
+    Parameters:
+    -----------
+    country: string or list.
+             String to get data for one country. List of strings to get data for
+             several countries. For example, country = ['United States', 'Australia'].
+    indicator: string or list.
+             String  to get data for one category. List of strings to get data for several calendar events.
+             For example, category = 'GDP Growth Rate' or 
+             category = ['Exports', 'Imports']
+    initDate: string with format: YYYY-MM-DD.
+             For example: '2011-01-01' 
+    endDate: string with format: YYYY-MM-DD.
+    output_type: string.
+             'dict'(default) for dictionary format output,
+             'raw' for list of dictionaries without any parsing.
+    Notes
+    ----- 
+    Must choose a country and an indicator.
+    Example
+    -------
+    getHistoricalData(country = 'United States', indicator = 'Imports', initDate = '2011-01-01', endDate = '2016-01-01')
+    getHistoricalData(country = ['United States', 'china'], indicator = ['Imports','Exports'], initDate = '2011-01-01', endDate = '2016-01-01')
+    """
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+
+    if type(country) is str and type(indicator) is str: 
+        linkAPI = 'https://api.tradingeconomics.com/historical/country/' + quote(country)  + '/indicator/' + quote(indicator) 
+    else:
+        linkAPI = paramCheck(country, indicator)
+        
+    if initDate == None and endDate == None:
+        minDate = [(datetime.now() - relativedelta(years=15)).strftime('%Y-%m-%d') ]
+        linkAPI = fn.finalLink(linkAPI, minDate) 
+    if initDate == None and (endDate is not None): 
+        raise DateError('initDate value is missing') 
+    if (initDate is not None) and (endDate is not None) :
+        try: 
+            fn.validate(initDate)
+        except ValueError:
+            raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
+        try: 
+            fn.validate(endDate)
+        except ValueError:
+            raise DateError ('Incorrect endDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
+        try:        
+            fn.validatePeriod(initDate, endDate)
+        except ValueError:
+            raise DateError ('Invalid time period.')
+        linkAPI = fn.finalLink(linkAPI, [initDate, endDate])
+    if (initDate is not None) and endDate == None :        
+        try: 
+            fn.validate(initDate)
+        except ValueError:
+            raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
+            if initDate > str(date.today()):
+                raise DateError ('Initial date out of range.')
+        linkAPI = fn.finalLink(linkAPI, [initDate])
+   
+    try:
+        linkAPI += '?c='+glob.apikey
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+    
+    try:
+        #print(linkAPI)
+        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
+    except Exception as e:
+        print(e)  
+        
+
+def getHistoricalRatings(country = None, rating = None, initDate = None, endDate=None, output_type = None):
+    """
+    Return historical information for specific country.
+    =================================================================
+    Parameters:
+    -----------
+    country: string or list.
+             String to get data for one country. List of strings to get data for
+             several countries. For example, country = ['United States', 'Australia'].
+        output_type: string.
+             'df'(default) for dictionary format output,
+             'raw' for list of dictionaries without any parsing.
+    Notes
+    ----- 
+    Without credentials only sample data will be provided.
+    Example
+    -------
+    getHistoricalRatings(country = 'United States', rating = None)
+    getHistoricalRatings(country = ['United States', 'United Kingdom'], rating = None)
+    getHistoricalRatings(country = 'United States', initDate ='2011-01-01')
+    getHistoricalRatings(country = 'United States', initDate ='2011-01-01', endDate = '2012-01-01')
+    
+    """
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+    
+    if country == None:
+        linkAPI = 'https://api.tradingeconomics.com/ratings/historical/'    
+    else:
+         linkAPI = checkCountryHistoricalRatings(country)
+        
+    if rating == None:
+        linkAPI = linkAPI
+    else:
+        linkAPI = checkRatings(linkAPI, rating)
+    if (country == None) and (rating == None):
+        linkAPI = 'https://api.tradingeconomics.com/ratings/historical/united%20states'   
+    else:
+        linkAPI = linkAPI
+    if (initDate is not None) and (endDate == None):
+        linkAPI = checkCountryHistoricalRatings(country) + "/" + initDate
+    elif (initDate is not None) and (endDate is not None):
+        linkAPI = checkCountryHistoricalRatings(country) + "/" + initDate + "/" + endDate
+    try:
+        linkAPI += '?c=' + glob.apikey
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+   
+    try:
+        #print(linkAPI)
+        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
+    except Exception as e:
+        print(e)   
+
+def getHistoricalByTicker(ticker=None, start_date=None, output_type=None):
+    """
+    Returns historical data by ticker.
+    =================================================================================
+    Parameters:
+    -----------
+        ticker: string.
+                ticker = 'USURTOT'
+        start_date: string.
+                start_date = '2015-03-01
+        output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+    Notes
+    -----
+    start_date is optional 
+    
+    Example
+    -------
+            getIndicatorByTicker(ticker = 'USURTOT', output_type = 'df')
+
+            getIndicatorByTicker(ticker = 'USURTOT', start_date = '2015-03-01, output_type = 'df')
+    """
+    
+    # d is a dictionary used for create the api url
+    d = {
+        'url_base': 'https://api.tradingeconomics.com/historical',
+        'country': '',
+        'ticker' : '',
+        'start_date': '',
+        'key': f'?c={glob.apikey}',
+        'output_type' : ''
+    }
+    if start_date :        
+        try: 
+            fn.validate(start_date)
+        except ValueError:
+            raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
+            
+
+    if ticker:
+        d['ticker']=f'/ticker/{fn.stringOrList(ticker)}'
+        d['start_date']=f'/{start_date}'
+        api_url_request = "%s%s%s%s" % (d['url_base'], d['ticker'],  d['start_date'],  d['key']) 
+        #print(api_url_request)
+        return fn.dataRequest(api_request=api_url_request, output_type=output_type)
+        #return
+         
+
+    return 'Ticker is required'
+
+
+def getHistoricalUpdates(output_type=None):
+    """
+    Returns historical Update.
+    =================================================================================
+    Parameters:
+    -----------
+        
+        output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+    Notes
+    -----
+    
+    
+    Example
+    -------
+            getHistoricalUpdates(output_type = 'df')
+
+
+    """
+    
+    # d is a dictionary used for create the api url
+    d = {
+        'url_base': 'https://api.tradingeconomics.com/historical/updates',
+        'key': f'?c={glob.apikey}',
+        'output_type' : ''
+    }
+    
+    api_url_request = "%s%s" % (d['url_base'], d['key']) 
+    #print(api_url_request)
+    return fn.dataRequest(api_request=api_url_request, output_type=output_type)
+
+    
+    
+         
+
+    
+
```

### Comparing `tradingeconomics-4.2.8/tradingeconomics/historicalDB.py` & `tradingeconomics-4.2.9/tradingeconomics/historicalDB.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-import json
-import itertools
-import urllib 
-import pandas as pd
-import sys
-from datetime import *
-from dateutil.relativedelta import relativedelta
-from . import functions as fn
-from . import glob
-import ssl
-
-PY3 = sys.version_info[0] == 3
-
-if PY3: # Python 3+
-    from urllib.request import urlopen
-    from urllib.parse import quote
-else: # Python 2.X
-    from urllib import urlopen
-    from urllib import quote
-
-class ParametersError(ValueError):
-    pass
-
-class DateError(ValueError):
-    pass
-
-class CredentialsError(ValueError):
-    pass
-
-class LoginError(AttributeError):
-    pass
-
-class WebRequestError(ValueError):
-    pass
-
-
-
-def getHistorical(symbol = None, initDate = None, endDate = None, output_type = None, *args): 
-    """
-    Return historical information for specific symbol.
-    =================================================================
-    Parameters:
-    -----------
-    symbol: string or list.
-             String to get data for one symbol. List of strings to get data for
-             several symbols. 
-            
-    output_type: string.
-             'dict'(default) for dictionary format output,
-             'raw' for list of dictionaries without any parsing.
-    Notes
-    ----- 
-    Must put symbol and type of data.
-    Example
-    -------
-    te.getHistorical("indu:ind", '2015-01-01')
-    te.getHistorical("indu:ind", '2015-01-01', '2017-01-01' )
-    te.getHistorical("USURTOT", '2015-01-01')
-    te.getHistorical(['aapl:us', 'indu:ind'])
-    te.getHistorical("USURTOT")
-    te.getHistorical("aapl:us")
-    te.getHistorical("are.fr.inr.rinr:worldbank")
-    te.getHistorical("RACEDISPARITY005007:fred")
-    te.getHistorical("PRTESP24031:comtrade")
-    """
-    linkAPI = 'https://api.tradingeconomics.com/'
- 
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-
-    if (symbol[-10:] == ':worldbank'):  
-        linkAPI += 'worldBank/historical?' + 's=' + quote(symbol[:-10], safe=':') 
-        
-    elif (symbol[-9:] == ':comtrade'):    
-        linkAPI += 'comtrade/historical/' +  quote(symbol[:-9], safe=':')  
-    
-    elif (symbol[-5:] == ':fred'):
-        linkAPI += 'fred/historical/' + quote(symbol[:-5], safe=':')          
-    
-    elif(':' not in symbol and type(symbol) is str):
-        linkAPI += 'historical/ticker/' + quote(symbol, safe='')
-                
-    elif (':' in symbol): 
-        linkAPI += 'markets/historical/' + quote(symbol, safe='') 
-    else:
-        linkAPI += 'markets/historical/' + quote(','.join(symbol), safe='')     
-    
-    if (initDate is not None) and (endDate is not None):
-        try: 
-            fn.validate(initDate)
-        except ValueError:
-            raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
-        try: 
-            fn.validate(endDate)
-        except ValueError:
-            raise DateError ('Incorrect endDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
-        try:        
-            fn.validatePeriod(initDate, endDate)
-        except ValueError:
-            raise DateError ('Invalid time period.')
-        linkAPI += '?d1=' + initDate + '&d2=' + endDate
-    
-    if (initDate is not None) and endDate == None :        
-        try: 
-            fn.validate(initDate)
-        except ValueError:
-            raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
-            if initDate > str(date.today()):
-                raise DateError ('Initial date out of range.')
-        if('markets' in linkAPI):
-            linkAPI += '?d1=' + initDate
-        else:
-            linkAPI += '/' + initDate
-        
-    if initDate == None and (endDate is not None):
-        initDate = (datetime.strptime(endDate, '%Y-%m-%d') - relativedelta(months=1)).strftime('%Y-%m-%d')
-        linkAPI += '?d1=' + initDate + '&d2=' + endDate
-
-    try:
-        if ('?' in linkAPI):
-            linkAPI += '&c='+glob.apikey 
-        else:   
-            linkAPI += '?c='+glob.apikey
-        
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-    try:
-        #print(linkAPI)
-        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
-    except Exception as e:
-        print(e) 
-            
-
+import json
+import itertools
+import urllib 
+import pandas as pd
+import sys
+from datetime import *
+from dateutil.relativedelta import relativedelta
+from . import functions as fn
+from . import glob
+import ssl
+
+PY3 = sys.version_info[0] == 3
+
+if PY3: # Python 3+
+    from urllib.request import urlopen
+    from urllib.parse import quote
+else: # Python 2.X
+    from urllib import urlopen
+    from urllib import quote
+
+class ParametersError(ValueError):
+    pass
+
+class DateError(ValueError):
+    pass
+
+class CredentialsError(ValueError):
+    pass
+
+class LoginError(AttributeError):
+    pass
+
+class WebRequestError(ValueError):
+    pass
+
+
+
+def getHistorical(symbol = None, initDate = None, endDate = None, output_type = None, *args): 
+    """
+    Return historical information for specific symbol.
+    =================================================================
+    Parameters:
+    -----------
+    symbol: string or list.
+             String to get data for one symbol. List of strings to get data for
+             several symbols. 
+            
+    output_type: string.
+             'dict'(default) for dictionary format output,
+             'raw' for list of dictionaries without any parsing.
+    Notes
+    ----- 
+    Must put symbol and type of data.
+    Example
+    -------
+    te.getHistorical("indu:ind", '2015-01-01')
+    te.getHistorical("indu:ind", '2015-01-01', '2017-01-01' )
+    te.getHistorical("USURTOT", '2015-01-01')
+    te.getHistorical(['aapl:us', 'indu:ind'])
+    te.getHistorical("USURTOT")
+    te.getHistorical("aapl:us")
+    te.getHistorical("are.fr.inr.rinr:worldbank")
+    te.getHistorical("RACEDISPARITY005007:fred")
+    te.getHistorical("PRTESP24031:comtrade")
+    """
+    linkAPI = 'https://api.tradingeconomics.com/'
+ 
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+
+    if (symbol[-10:] == ':worldbank'):  
+        linkAPI += 'worldBank/historical?' + 's=' + quote(symbol[:-10], safe=':') 
+        
+    elif (symbol[-9:] == ':comtrade'):    
+        linkAPI += 'comtrade/historical/' +  quote(symbol[:-9], safe=':')  
+    
+    elif (symbol[-5:] == ':fred'):
+        linkAPI += 'fred/historical/' + quote(symbol[:-5], safe=':')          
+    
+    elif(':' not in symbol and type(symbol) is str):
+        linkAPI += 'historical/ticker/' + quote(symbol, safe='')
+                
+    elif (':' in symbol): 
+        linkAPI += 'markets/historical/' + quote(symbol, safe='') 
+    else:
+        linkAPI += 'markets/historical/' + quote(','.join(symbol), safe='')     
+    
+    if (initDate is not None) and (endDate is not None):
+        try: 
+            fn.validate(initDate)
+        except ValueError:
+            raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
+        try: 
+            fn.validate(endDate)
+        except ValueError:
+            raise DateError ('Incorrect endDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
+        try:        
+            fn.validatePeriod(initDate, endDate)
+        except ValueError:
+            raise DateError ('Invalid time period.')
+        linkAPI += '?d1=' + initDate + '&d2=' + endDate
+    
+    if (initDate is not None) and endDate == None :        
+        try: 
+            fn.validate(initDate)
+        except ValueError:
+            raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
+            if initDate > str(date.today()):
+                raise DateError ('Initial date out of range.')
+        if('markets' in linkAPI):
+            linkAPI += '?d1=' + initDate
+        else:
+            linkAPI += '/' + initDate
+        
+    if initDate == None and (endDate is not None):
+        initDate = (datetime.strptime(endDate, '%Y-%m-%d') - relativedelta(months=1)).strftime('%Y-%m-%d')
+        linkAPI += '?d1=' + initDate + '&d2=' + endDate
+
+    try:
+        if ('?' in linkAPI):
+            linkAPI += '&c='+glob.apikey 
+        else:   
+            linkAPI += '?c='+glob.apikey
+        
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+    try:
+        #print(linkAPI)
+        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
+    except Exception as e:
+        print(e) 
+            
+
```

### Comparing `tradingeconomics-4.2.8/tradingeconomics/historicalEurostat.py` & `tradingeconomics-4.2.9/tradingeconomics/historicalEurostat.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-import json
-import itertools
-import urllib 
-import pandas as pd
-import sys
-from datetime import *
-from dateutil.relativedelta import relativedelta
-from . import functions as fn
-from . import glob
-import ssl
-
-PY3 = sys.version_info[0] == 3
-
-if PY3: # Python 3+
-    from urllib.request import urlopen
-    from urllib.parse import quote
-else: # Python 2.X
-    from urllib import urlopen
-    from urllib import quote
-
-class ParametersError(ValueError):
-    pass
-
-class DateError(ValueError):
-    pass
-
-class CredentialsError(ValueError):
-    pass
-
-class LoginError(AttributeError):
-    pass
-
-class WebRequestError(ValueError):
-    pass
-
-def getID(ID):
-    linkAPI = 'https://api.tradingeconomics.com/eurostat/historical/'
-    if type(ID) is str:
-        linkAPI += quote(ID)
-    else:
-        linkAPI += quote(",".join(ID), safe='') 
-    return linkAPI
-
-def getHistoricalEurostat(ID = None, initDate = None, endDate=None, output_type = None):
-    """
-    Return historical Eurostat data.
-    =================================================================
-    Parameters:
-    -----------
-    ID: string.
-             String to get data for particular ID.
-             For example, ID = '24804'.
-    initDate: string.
-             String to get data by start date.
-             For example, initDate = '2015-01-01'.
-    endDate: string.
-             String to get data by start date.
-             For example, endDate = '2020-01-01'.
-    output_type: string.
-            'df'(default) for dictionary format output,
-            'raw' for list of dictionaries without any parsing.
-    Notes
-    ----- 
-    Without credentials only sample data will be provided.
-    Example
-    -------
-    getHistoricalEurostat(ID = '24804', output_type = 'df')
-    getHistoricalEurostat(ID = '24804', initDate ='2015-01-01', output_type = 'df')
-    getHistoricalEurostat(ID = '24804', initDate ='2015-01-01', endDate = '2020-01-01', output_type = 'df')
-    
-    """
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-    
-    if ID == None:
-        raise ValueError ('An ID needs to be supplied.')
-    if ID != None:
-        linkAPI = getID(ID)    
-    if (initDate is not None) and (endDate == None):
-        linkAPI = getID(ID)  + "?d1=" + initDate
-    elif (initDate is not None) and (endDate is not None):
-        linkAPI = getID(ID)  + "?d1=" + initDate + "&d2=" + endDate
-    
-    try:
-        if (initDate)is not None or (endDate) is not None:
-            linkAPI += '&c=' + glob.apikey
-        else:
-            linkAPI += '?c=' + glob.apikey
-        #print(linkAPI)
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-   
-    try:
-        #print(linkAPI)
-        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
-    except Exception as e:
+import json
+import itertools
+import urllib 
+import pandas as pd
+import sys
+from datetime import *
+from dateutil.relativedelta import relativedelta
+from . import functions as fn
+from . import glob
+import ssl
+
+PY3 = sys.version_info[0] == 3
+
+if PY3: # Python 3+
+    from urllib.request import urlopen
+    from urllib.parse import quote
+else: # Python 2.X
+    from urllib import urlopen
+    from urllib import quote
+
+class ParametersError(ValueError):
+    pass
+
+class DateError(ValueError):
+    pass
+
+class CredentialsError(ValueError):
+    pass
+
+class LoginError(AttributeError):
+    pass
+
+class WebRequestError(ValueError):
+    pass
+
+def getID(ID):
+    linkAPI = 'https://api.tradingeconomics.com/eurostat/historical/'
+    if type(ID) is str:
+        linkAPI += quote(ID)
+    else:
+        linkAPI += quote(",".join(ID), safe='') 
+    return linkAPI
+
+def getHistoricalEurostat(ID = None, initDate = None, endDate=None, output_type = None):
+    """
+    Return historical Eurostat data.
+    =================================================================
+    Parameters:
+    -----------
+    ID: string.
+             String to get data for particular ID.
+             For example, ID = '24804'.
+    initDate: string.
+             String to get data by start date.
+             For example, initDate = '2015-01-01'.
+    endDate: string.
+             String to get data by start date.
+             For example, endDate = '2020-01-01'.
+    output_type: string.
+            'df'(default) for dictionary format output,
+            'raw' for list of dictionaries without any parsing.
+    Notes
+    ----- 
+    Without credentials only sample data will be provided.
+    Example
+    -------
+    getHistoricalEurostat(ID = '24804', output_type = 'df')
+    getHistoricalEurostat(ID = '24804', initDate ='2015-01-01', output_type = 'df')
+    getHistoricalEurostat(ID = '24804', initDate ='2015-01-01', endDate = '2020-01-01', output_type = 'df')
+    
+    """
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+    
+    if ID == None:
+        raise ValueError ('An ID needs to be supplied.')
+    if ID != None:
+        linkAPI = getID(ID)    
+    if (initDate is not None) and (endDate == None):
+        linkAPI = getID(ID)  + "?d1=" + initDate
+    elif (initDate is not None) and (endDate is not None):
+        linkAPI = getID(ID)  + "?d1=" + initDate + "&d2=" + endDate
+    
+    try:
+        if (initDate)is not None or (endDate) is not None:
+            linkAPI += '&c=' + glob.apikey
+        else:
+            linkAPI += '?c=' + glob.apikey
+        #print(linkAPI)
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+   
+    try:
+        #print(linkAPI)
+        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
+    except Exception as e:
         print(e)
```

### Comparing `tradingeconomics-4.2.8/tradingeconomics/historicalMarkets.py` & `tradingeconomics-4.2.9/tradingeconomics/historicalMarkets.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-import json
-import itertools
-import urllib 
-import pandas as pd
-import sys
-from datetime import *
-from dateutil.relativedelta import relativedelta
-from . import functions as fn
-from . import glob
-import ssl
-
-PY3 = sys.version_info[0] == 3
-
-if PY3: # Python 3+
-    from urllib.request import urlopen
-    from urllib.parse import quote
-else: # Python 2.X
-    from urllib import urlopen
-    from urllib import quote
-
-class ParametersError(ValueError):
-    pass
-
-class DateError(ValueError):
-    pass
-
-class CredentialsError(ValueError):
-    pass
-
-class LoginError(AttributeError):
-    pass
-
-class WebRequestError(ValueError):
-    pass
-
-def parseData(data):
-    datafr = pd.DataFrame.from_dict(data)
-    datafr['dates'] = pd.to_datetime(datafr['dates'], format='%d/%m/%Y' )
-    indx = datafr['dates']
-    datafr = datafr[['symbol','open', 'high', 'low', 'close']]
-    datafr = datafr.set_index(indx)
-    datafr.index.name = None
-    #del datafr.index.name
-    return datafr    
-    
-    
-def fetchMarkets(symbol = None, initDate=None, endDate=None, output_type=None):
-    """
-    Return historical information for specific markets symbol.
-    =================================================================
-
-    Parameters:
-    -----------
-    symbol: Unique symbol used by TradingEconomics. 
-             For example: 'aapl:us'
-    initDate: string with format: YYYY-MM-DD.
-             For example: '2011-01-01' 
-    endDate: string with format: YYYY-MM-DD.
-    output_type: string.
-             'dict'(default) for dictionary format output,
-             'df' for dataframe,
-             'raw' for list of dictionaries without any parsing.
-
-    Notes
-    ----- 
-    A symbol must be provided.
-
-    Example
-    -------
-    fetchMarkets(symbol = 'indu:ind')
-    fetchMarkets(symbol = 'indu:ind', initDate = '2017-01-01', endDate = '2017-06-15', output_type='raw')
-    fetchMarkets(symbol = ['aapl:us', 'indu:ind'], initDate = '2017-01-01', endDate = '2017-06-15')
-    """
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-
-    linkAPI = 'https://api.tradingeconomics.com/markets/historical/'
-    
-    
-    if type(symbol) is not str:        
-        linkAPI = 'https://api.tradingeconomics.com/markets/historical/' + quote(",".join(symbol), safe='') 
-    else:   
-        linkAPI = 'https://api.tradingeconomics.com/markets/historical/' + quote(symbol, safe='')
-    
-    try:
-        linkAPI += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-
-    if (initDate is not None) and (endDate is not None) :
-        try: 
-            fn.validate(initDate)
-        except ValueError:
-            raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
-        try: 
-            fn.validate(endDate)
-        except ValueError:
-            raise DateError ('Incorrect endDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
-        try:        
-            fn.validatePeriod(initDate, endDate)
-        except ValueError:
-            raise DateError ('Invalid time period.')
-        linkAPI += '&d1=' + initDate + '&d2=' + endDate
-    
-    elif (initDate is not None) and endDate == None :        
-        try: 
-            fn.validate(initDate)
-        except ValueError:
-            raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
-            if initDate > str(date.today()):
-                raise DateError ('Initial date out of range.')
-        linkAPI += '&d1=' + initDate
-    
-    elif initDate == None and (endDate is not None):
-        initDate = (datetime.strptime(endDate, '%Y-%m-%d') - relativedelta(months=1)).strftime('%Y-%m-%d')
-        linkAPI += '&d1=' + initDate + '&d2=' + endDate   
-    
-    try:
-        #print(linkAPI)
-        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
-    except Exception as e:
-        print(e) 
-            
-
+import json
+import itertools
+import urllib 
+import pandas as pd
+import sys
+from datetime import *
+from dateutil.relativedelta import relativedelta
+from . import functions as fn
+from . import glob
+import ssl
+
+PY3 = sys.version_info[0] == 3
+
+if PY3: # Python 3+
+    from urllib.request import urlopen
+    from urllib.parse import quote
+else: # Python 2.X
+    from urllib import urlopen
+    from urllib import quote
+
+class ParametersError(ValueError):
+    pass
+
+class DateError(ValueError):
+    pass
+
+class CredentialsError(ValueError):
+    pass
+
+class LoginError(AttributeError):
+    pass
+
+class WebRequestError(ValueError):
+    pass
+
+def parseData(data):
+    datafr = pd.DataFrame.from_dict(data)
+    datafr['dates'] = pd.to_datetime(datafr['dates'], format='%d/%m/%Y' )
+    indx = datafr['dates']
+    datafr = datafr[['symbol','open', 'high', 'low', 'close']]
+    datafr = datafr.set_index(indx)
+    datafr.index.name = None
+    #del datafr.index.name
+    return datafr    
+    
+    
+def fetchMarkets(symbol = None, initDate=None, endDate=None, output_type=None):
+    """
+    Return historical information for specific markets symbol.
+    =================================================================
+
+    Parameters:
+    -----------
+    symbol: Unique symbol used by TradingEconomics. 
+             For example: 'aapl:us'
+    initDate: string with format: YYYY-MM-DD.
+             For example: '2011-01-01' 
+    endDate: string with format: YYYY-MM-DD.
+    output_type: string.
+             'dict'(default) for dictionary format output,
+             'df' for dataframe,
+             'raw' for list of dictionaries without any parsing.
+
+    Notes
+    ----- 
+    A symbol must be provided.
+
+    Example
+    -------
+    fetchMarkets(symbol = 'indu:ind')
+    fetchMarkets(symbol = 'indu:ind', initDate = '2017-01-01', endDate = '2017-06-15', output_type='raw')
+    fetchMarkets(symbol = ['aapl:us', 'indu:ind'], initDate = '2017-01-01', endDate = '2017-06-15')
+    """
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+
+    linkAPI = 'https://api.tradingeconomics.com/markets/historical/'
+    
+    
+    if type(symbol) is not str:        
+        linkAPI = 'https://api.tradingeconomics.com/markets/historical/' + quote(",".join(symbol), safe='') 
+    else:   
+        linkAPI = 'https://api.tradingeconomics.com/markets/historical/' + quote(symbol, safe='')
+    
+    try:
+        linkAPI += '?c=' + glob.apikey
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+
+    if (initDate is not None) and (endDate is not None) :
+        try: 
+            fn.validate(initDate)
+        except ValueError:
+            raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
+        try: 
+            fn.validate(endDate)
+        except ValueError:
+            raise DateError ('Incorrect endDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
+        try:        
+            fn.validatePeriod(initDate, endDate)
+        except ValueError:
+            raise DateError ('Invalid time period.')
+        linkAPI += '&d1=' + initDate + '&d2=' + endDate
+    
+    elif (initDate is not None) and endDate == None :        
+        try: 
+            fn.validate(initDate)
+        except ValueError:
+            raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
+            if initDate > str(date.today()):
+                raise DateError ('Initial date out of range.')
+        linkAPI += '&d1=' + initDate
+    
+    elif initDate == None and (endDate is not None):
+        initDate = (datetime.strptime(endDate, '%Y-%m-%d') - relativedelta(months=1)).strftime('%Y-%m-%d')
+        linkAPI += '&d1=' + initDate + '&d2=' + endDate   
+    
+    try:
+        #print(linkAPI)
+        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
+    except Exception as e:
+        print(e) 
+            
+
```

### Comparing `tradingeconomics-4.2.8/tradingeconomics/markets.py` & `tradingeconomics-4.2.9/tradingeconomics/markets.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,643 +1,653 @@
-import json 
-import urllib 
-import pandas as pd
-import sys
-from datetime import *
-from . import glob
-import ssl
-from . import functions as fn
-from dateutil.relativedelta import relativedelta
-
-PY3 = sys.version_info[0] == 3
-
-if PY3: # Python 3+
-    from urllib.request import urlopen
-    from urllib.parse import quote
-else: # Python 2.X
-    from urllib import urlopen
-    from urllib import quote
-
-
-class ParametersError(ValueError):
-    pass
-
-class CredentialsError(ValueError):
-    pass
-
-class LoginError(AttributeError):
-    pass
-
-class DateError(ValueError):
-    pass
-
-class WebRequestError(ValueError):
-    pass
-
-def checkPage(linkAPI, page):
-    if page != None:
-        linkAPI += '&page={0}'.format(page)
-    return linkAPI
-
-def checkCategory(linkAPI, category):
-    if type(category) is str:
-        linkAPI += '?category=' + quote (category, safe='')
-    else:
-        linkAPI += '?category=' + quote(",".join(category), safe="")
-    return linkAPI
-   
-   
-def getMarketsData(marketsField, output_type=None):
-    """
-    Returns a list of available commodities, currencies, indexes or 
-    bonds and their latest values.
-    ==========================================================
-    Parameters:
-    -----------
-    marketsField: string.
-            Takes either one of 'commodity','currency',
-            'index' or 'bond' as options.
-             
-    output_type: string.
-             'dict'(default), 'df' for data frame,
-             'raw' for list of unparsed data. 
-    Example
-    -------
-    getMarketsData(marketsField = 'index')
-    """
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-        
-    fields =['commodities', 'currency', 'index', 'bond', 'crypto']
-    if marketsField not in fields:
-        raise ParametersError ('Accepted values for marketsField are \'commodities\', \'currency\', \'index\', \'crypto\' or \'bond\'.')
-    linkAPI = 'https://api.tradingeconomics.com/markets/' + quote(marketsField, safe='') 
-    try:
-        linkAPI += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-
-    try:
-      output = fn.dataRequest(linkAPI, output_type)
-      return output
-    except ValueError:
-      raise WebRequestError ('Something went wrong.')  
-    
-    
-
-def getCurrencyCross(cross, output_type=None):
-    """
-    Returns a list of latest values available for 
-    currencies and the chosen cross.
-    ==========================================================
-    Parameters:
-    -----------
-    cross: string.
-            
-    output_type: string.
-             'dict'(default), 'df' for data frame,
-             'raw' for list of unparsed data. 
-    Example
-    -------
-    getCurrencyCross(cross = 'EUR')
-    getCurrencyCross(cross = 'EUR', output_type='df')
-    """
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-        
-    
-    if cross is not None:       
-        linkAPI = 'https://api.tradingeconomics.com/markets/currency?cross=' + quote(cross, safe='') 
-    else:
-        raise ParametersError ('You must provide a cross for your currency pair')
-    try:
-        linkAPI += '&c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-    
-    try:
-      output = fn.dataRequest(linkAPI, output_type)
-      return output
-    except ValueError:
-      raise WebRequestError ('Something went wrong.')  
-    
-    
-
-
-def getMarketsBySymbol(symbols, output_type=None):
-    """
-    Returns a markets information for specific symbols.
-    ==========================================================
-    Parameters:
-    -----------
-    symbols: string or list.
-            String to get data for symbol. List of strings to get data for
-             several symbols. For example, symbols = ['aapl:us', 'indu:ind'].
-             
-    output_type: string.
-             'dict'(default), 'df' for data frame,
-             'raw' for list of unparsed data. 
-    Example
-    -------
-    getMarketsBySymbol(symbols = 'indu:ind')
-    getMarketsBySymbol(symbols = ['aapl:us', 'indu:ind'], output_type = 'raw')
-    """
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-
-    if type(symbols) is not str:        
-        linkAPI = 'https://api.tradingeconomics.com/markets/symbol/' + quote(",".join(symbols), safe='') 
-    else:   
-        linkAPI = 'https://api.tradingeconomics.com/markets/symbol/' + quote(symbols, safe='')
-    
-    try:
-        linkAPI += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-    
-    try:
-      output = fn.dataRequest(linkAPI, output_type)
-      return output
-    except ValueError:
-      raise WebRequestError ('Something went wrong.')  
-
-
-def getMarketsIntraday(symbols, initDate=None, endDate=None, output_type=None):
-    """
-    Returns a markets intraday information for specific symbols.
-    ==========================================================
-    Parameters:
-    -----------
-    symbols: string or list.
-            String to get data for symbol. List of strings to get data for
-             several symbols. For example, symbols = ['aapl:us', 'indu:ind'].
-    
-    initDate: string with format: YYYY-MM-DD.
-             For example: '2011-01-01' 
-    endDate: string with format: YYYY-MM-DD.    
-    output_type: string.
-             'dict'(default), 'df' for data frame,
-             'raw' for list of unparsed data. 
-    Example
-    -------
-    getMarketsIntraday(symbols = 'indu:ind')
-    getMarketsIntraday(symbols = 'indu:ind', initDate='2018-03-13 15:30')
-    getMarketsIntraday(symbols = ['aapl:us', 'indu:ind'], initDate='2022-01-01', endDate='2022-12-31', output_type = 'raw')
-    """
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-
-    if type(symbols) is not str:        
-        linkAPI = 'https://api.tradingeconomics.com/markets/intraday/' + quote(",".join(symbols), safe='') 
-    else:   
-        linkAPI = 'https://api.tradingeconomics.com/markets/intraday/' + quote(symbols, safe='')
-    
-    try:
-        linkAPI += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-    
-    linkAPI = fn.checkDates(linkAPI, initDate, endDate)
-
-    try:
-      output = fn.dataRequest(linkAPI, output_type)
-      return output
-    except ValueError:
-      raise WebRequestError ('Something went wrong.')  
-
-def getMarketsPeers(symbols, output_type = None):
-    """
-    Returns a markets peers information for specific symbols.
-    ==========================================================
-    Parameters:
-    -----------
-    symbols: string or list.
-            String to get data for symbol. List of strings to get data for
-             several symbols. For example, symbols = ['aapl:us', 'indu:ind'].
-             
-    output_type: string.
-             'dict'(default), 'df' for data frame,
-             'raw' for list of unparsed data. 
-    Example
-    -------
-    getMarketsPeers(symbols = 'indu:ind')
-    getMarketsPeers(symbols = ['aapl:us', 'indu:ind'], output_type = 'raw')
-    """
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-
-    if type(symbols) is not str:        
-        linkAPI = 'https://api.tradingeconomics.com/markets/peers/' + quote(",".join(symbols), safe='') 
-    else:   
-        linkAPI = 'https://api.tradingeconomics.com/markets/peers/' + quote(symbols, safe='')
-    
-    try:
-        linkAPI += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-    try:
-      output = fn.dataRequest(linkAPI, output_type)
-      return output
-    except ValueError:
-      raise WebRequestError ('Something went wrong.')  
-
-def getMarketsComponents(symbols, output_type = None):
-    """
-    Returns a stock market index components information for specific symbols.
-    ==========================================================
-    Parameters:
-    -----------
-    symbols: string or list.
-            String to get data for symbol. List of strings to get data for
-             several symbols. For example, symbols = ['aapl:us', 'indu:ind'].
-             
-    output_type: string.
-             'dict'(default), 'df' for data frame,
-             'raw' for list of unparsed data. 
-    Example
-    -------
-    getMarketsComponents(symbols = 'psi20:ind')
-    getMarketsComponents(symbols = ['psi20:ind', 'indu:ind'], output_type = 'raw')
-    """
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-
-    if type(symbols) is not str:        
-        linkAPI = 'https://api.tradingeconomics.com/markets/components/' + quote(",".join(symbols), safe='') 
-    else:   
-        linkAPI = 'https://api.tradingeconomics.com/markets/components/' + quote(symbols, safe='')
-    
-    try:
-        linkAPI += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-    try:
-      output = fn.dataRequest(linkAPI, output_type)
-      return output
-    except ValueError:
-      raise WebRequestError ('Something went wrong.')  
-
-def getMarketsSearch(country=None, category = None, page = None, output_type = None):    
-    """
-    Search for country, category and page number.
-    ==========================================================
-    Parameters:
-    -----------
-    symbols: string.
-            String to get data for country and category. 
-    
-    output_type: string.
-             'dict'(default), 'df' for data frame,
-             'raw' for list of unparsed data. 
-    Example
-    -------
-    getMarketsSearch(country = 'japan', category = None, page = None, output_type = None)
-    getMarketsSearch(country = 'japan', category = 'index', page = None, output_type = None)
-    getMarketsSearch(country = 'japan', category = ['index', 'markets'], page = None, output_type = None)
-    getMarketsSearch(country = 'japan', category = 'index', page = None, output_type = None)
-    """
-    
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-
-    if type(country) is not str:        
-        linkAPI = 'https://api.tradingeconomics.com/markets/search/' + quote(",".join(country), safe='') 
-    else:   
-        linkAPI = 'https://api.tradingeconomics.com/markets/search/' + quote(country, safe='')
-    if (category) is not None:    
-        linkAPI = checkCategory(linkAPI, category)       
-    if (page) is not None:
-        linkAPI = checkPage(linkAPI, page)
-    
-    try:
-        if (category)is not None:
-            linkAPI += '&c=' + glob.apikey
-        else:
-            linkAPI += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-    
-    try:
-      output = fn.dataRequest(linkAPI, output_type)
-      return output
-    except ValueError:
-      raise WebRequestError ('Something went wrong.')  
-
-
-def getMarketsForecasts(category=None, symbol=None,  output_type = None):
-    """
-    Returns a stock market forecast information for specific symbols and categories.
-    ================================================================================
-    Parameters:
-    -----------
-    symbol: string or list.
-            String to get data for symbol. List of strings to get data for
-             several symbols. For example, symbols = ['aapl:us', 'indu:ind'].
-    category: string.
-            String to get data by category.  
-            For example, category = 'index'         
-             
-    output_type: string.
-             'dict'(default), 'df' for data frame,
-             'raw' for list of unparsed data. 
-    Example
-    -------
-    getMarketsForecasts(category = 'bond')
-    getMarketsForecasts(symbol = ['psi20:ind', 'indu:ind'], output_type = 'df')
-    getMarketsForecasts(symbol =  'indu:ind', output_type = 'df')
-    """
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context    
-  
-    if type(symbol) is list: 
-        linkAPI = 'http://api.tradingeconomics.com/markets/forecasts' + '/symbol/' + quote(",".join(symbol), safe='') 
-             
-    else:  
-       linkAPI = 'http://api.tradingeconomics.com/markets/forecasts' + '/symbol/' + quote(str(symbol)) 
-    
-    if category is not None:
-        linkAPI = 'http://api.tradingeconomics.com/markets/forecasts/' + quote(category)
-       
-
-    try:
-        linkAPI += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-    
-    try:
-    #   output = fn.makeRequestAndParse(linkAPI, output_type)
-      output = fn.dataRequest(linkAPI, output_type)
-      return output
-    except ValueError:
-      raise WebRequestError ('Something went wrong.')   
-
-
-def getMarketsIntradayByInterval(symbol, interval, initDate,endDate,output_type=None):
-    """
-    Returns Aggregate intraday prices by interval - allowed intervals: 1m, 5m, 10m, 15m, 30m, 1h, 2h, 4h.
-    =================================================================================
-    Parameters:
-    -----------
-        symbol: string.
-                symbol = 'CL1:COM'
-                symbol = ['CL1:COM','AAPL:US']
-        interval: string
-                interval='1m'
-        initDate: string.
-                initDate = '2021-01-01'
-        endDate:string.
-                endDate = '2021-01-10'
-        
-        output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web. 
-    Notes
-    -----
-    
-    
-    Example
-    -------
-            getMarketsIntradayByInterval(symbol='CL1:COM',interval='1m',initDate='2022-01-01',endDate='2023-12-01',output_type='df')
-            getMarketsIntradayByInterval(symbol=['CL1:COM','AAPL:US'],interval='1m',initDate='2022-01-01',endDate='2022-12-01',output_type='df')
-    """
-            
-    
-    # d is a dictionary used for create the api url
-    d = {
-        'url_base': 'https://api.tradingeconomics.com/markets/intraday',
-        'symbol': f'/{fn.stringOrList(symbol)}',
-        'interval' : f'?agr={fn.stringOrList(interval)}',
-        'init_date': '',
-        'end_date':'',
-        'key': f'&client={glob.apikey}',
-        'output_type' : ''
-    }
-    if initDate and endDate :     
-
-        fn.validate(initDate)
-        fn.validate(endDate)
-        fn.validatePeriod(initDate, endDate)
-        # #it will parse endDate when initDate and endData are the same. 
-        # endDate = (lambda x, y : f"{endDate[0:8]}{(int(endDate[8:])+1)}" if x==y else endDate)(initDate,endDate)
-        # d['init_date']=f'&d1={initDate}'
-        # d['end_date']=f'&d2={endDate}'
-
-    
-
-    api_url_request = "%s%s%s%s%s%s" % (d['url_base'], d['symbol'], d['interval'],  d['init_date'],  d['end_date'],  d['key']) 
-
-    try:
-      # print(api_url_request)
-      output = fn.dataRequest(api_url_request, output_type)
-      return output
-    except ValueError:
-      raise WebRequestError ('Something went wrong.')   
-    
-
-
-def getMarketsStockDescriptions(symbol = None,country = None, output_type=None):
-    """
-    Returns Markets Descriptions
-    =================================================================================
-    Parameters:
-    -----------
-        symbol: string or list.
-                symbol = 'AAPL:US'
-                symbol = ['AAPL:US','FB:US']
-        
-        country: string or list
-                country = 'france'
-                countr = ['france','portugal']
-        
-        
-        output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web. 
-    Notes
-    -----
-    
-    
-    Example
-    -------
-            getMarketsStockDescriptions(symbol='AAPL:US',output_type='df')
-            getMarketsStockDescriptions(symbol=['AAPL:US','FB:US'],output_type='df')
-            getMarketsStockDescriptions(country='france',output_type='df')
-            getMarketsStockDescriptions(country=['france','portugal'],output_type='df')
-    """
-            
-    # url example: 'https://api.tradingeconomics.com/markets/stockdescriptions/symbol/aapl:us,fb:us?c=guest:guest'
-    # https://api.tradingeconomics.com/markets/stockdescriptions/country/france,portugal?c=guest:guest
-
-    # d is a dictionary used for create the api url
-    d = {
-        'url_base': 'https://api.tradingeconomics.com/markets/stockdescriptions',
-        'symbol': '',
-        'country': '',
-        'key': f'?c={glob.apikey}',
-        'output_type' : ''
-    }
-
-    if symbol:
-        d['symbol'] = f'/symbol/{(fn.stringOrList(symbol))}'
-    
-    if country:
-        d['country'] = f'/country/{(fn.stringOrList(country))}'
-
-    if country and symbol or country is None and symbol is None:
-        return 'You have to pass country or symbol'
-    
-    
-
-    api_url_request = "%s%s%s%s" % (d['url_base'], d['symbol'],d['country'],  d['key']) 
-    try:
-      output = fn.dataRequest(api_url_request, output_type)
-      return output
-    except ValueError:
-      raise WebRequestError ('Something went wrong.')   
-
-def getMarketsSymbology(symbol = None,ticker = None, isin=None,output_type=None):
-    """
-    Returns Markets Descriptions
-    =================================================================================
-    Parameters:
-    -----------
-        symbol: string 
-                symbol = 'AAPL:US'
-                
-        
-        ticker: string 
-                ticker = 'aapl'
-                
-        
-        
-        output_type: string.
-            'dict'(default) for dictionary format output, 'df' for data frame,
-            'raw' for list of dictionaries directly from the web. 
-    Notes
-    -----
-    
-    
-    Example
-    -------
-            getMarketsSymbology(symbol='AAPL:US',output_type='df')
-            getMarketsSymbology(ticker='aapl',output_type='df')
-            getMarketsSymbology(isin='US0378331005',output_type='df')
-            
-    """
-    #validateParameters
-    parametersList = []
-    (lambda x : parametersList.append(x) if x != None else None )(symbol) 
-    (lambda x : parametersList.append(x) if x != None else None )(ticker) 
-    (lambda x : parametersList.append(x) if x != None else None )(isin) 
-
-    if len(parametersList) > 1:
-      print('Only one argument must be provided for each request')
-      return 
-          
-
-    # d is a dictionary used for create the api url
-    d = {
-        'url_base': 'https://api.tradingeconomics.com/markets/symbology',
-        'symbol': '',
-        'ticker': '',
-        'isin': '',
-        'key': f'?c={glob.apikey}',
-        'output_type' : ''
-    }
-
-
-    if symbol:
-        d['symbol'] = f'/symbol/{(fn.stringOrList(symbol))}'
-    
-    if ticker:
-        d['ticker'] = f'/ticker/{(fn.stringOrList(ticker))}'
-    
-    if isin:
-        d['isin'] = f'/isin/{(fn.stringOrList(isin))}'
-
-    api_url_request = "%s%s%s%s%s" % (d['url_base'], d['symbol'],d['ticker'],  d['isin'],d['key']) 
-    try:
-      output = fn.dataRequest(api_url_request, output_type)
-      return output
-    except ValueError:
-      raise WebRequestError ('Something went wrong.')   
-
-def getStocksByCountry (country:str,output_type=None):
-    """
-    Returns Stocks List to a specific country
-    =================================================================================
-    Parameters:
-    -----------
-        country: string 
-                symbol = 'United States'
-                
-        output_type: string.
-            'dict'(default) for dictionary format output, 'df' for data frame,
-            'raw' for list of dictionaries directly from the web. 
-    Notes
-    -----
-    
-    
-    Example
-    -------
-            getStocksByCountry(country='United States',output_type='df')
-            
-    """
-    
-          
-
-    # d is a dictionary used for create the api url
-    d = {
-        'url_base': 'https://api.tradingeconomics.com/markets/country/',
-        'country': '',
-        'key': f'?c={glob.apikey}',
-        'output_type' : ''
-    }
-
-    try:
-        if type(country) == str:
-            d['country'] = f'{quote(country)}'
-        else:
-          raise AttributeError ('country must be a string')
-    except Exception as e:
-      raise e
-    
-    
-
-    api_url_request = "%s%s%s" % (d['url_base'], d['country'],d['key']) 
-    try:
-      output = fn.dataRequest(api_url_request, output_type)
-      return output
-    except ValueError:
+import json 
+import urllib 
+import pandas as pd
+import sys
+from datetime import *
+from . import glob
+import ssl
+from . import functions as fn
+from dateutil.relativedelta import relativedelta
+
+PY3 = sys.version_info[0] == 3
+
+if PY3: # Python 3+
+    from urllib.request import urlopen
+    from urllib.parse import quote
+else: # Python 2.X
+    from urllib import urlopen
+    from urllib import quote
+
+
+class ParametersError(ValueError):
+    pass
+
+class CredentialsError(ValueError):
+    pass
+
+class LoginError(AttributeError):
+    pass
+
+class DateError(ValueError):
+    pass
+
+class WebRequestError(ValueError):
+    pass
+
+def checkPage(linkAPI, page):
+    if page != None:
+        linkAPI += '&page={0}'.format(page)
+    return linkAPI
+
+def checkCategory(linkAPI, category):
+    if type(category) is str:
+        linkAPI += '?category=' + quote (category, safe='')
+    else:
+        linkAPI += '?category=' + quote(",".join(category), safe="")
+    return linkAPI
+   
+   
+def getMarketsData(marketsField, output_type=None):
+    """
+    Returns a list of available commodities, currencies, indexes or 
+    bonds and their latest values.
+    ==========================================================
+    Parameters:
+    -----------
+    marketsField: string.
+            Takes either one of 'commodity','currency',
+            'index' or 'bond' as options.
+             
+    output_type: string.
+             'dict'(default), 'df' for data frame,
+             'raw' for list of unparsed data. 
+    Example
+    -------
+    getMarketsData(marketsField = 'index')
+    """
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+        
+    fields =['commodities', 'currency', 'index', 'bond', 'crypto']
+    if marketsField not in fields:
+        raise ParametersError ('Accepted values for marketsField are \'commodities\', \'currency\', \'index\', \'crypto\' or \'bond\'.')
+    linkAPI = 'https://api.tradingeconomics.com/markets/' + quote(marketsField, safe='') 
+    try:
+        linkAPI += '?c=' + glob.apikey
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+
+    try:
+      output = fn.dataRequest(linkAPI, output_type)
+      return output
+    except ValueError:
+      raise WebRequestError ('Something went wrong.')  
+    
+    
+
+def getCurrencyCross(cross, output_type=None):
+    """
+    Returns a list of latest values available for 
+    currencies and the chosen cross.
+    ==========================================================
+    Parameters:
+    -----------
+    cross: string.
+            
+    output_type: string.
+             'dict'(default), 'df' for data frame,
+             'raw' for list of unparsed data. 
+    Example
+    -------
+    getCurrencyCross(cross = 'EUR')
+    getCurrencyCross(cross = 'EUR', output_type='df')
+    """
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+        
+    
+    if cross is not None:       
+        linkAPI = 'https://api.tradingeconomics.com/markets/currency?cross=' + quote(cross, safe='') 
+    else:
+        raise ParametersError ('You must provide a cross for your currency pair')
+    try:
+        linkAPI += '&c=' + glob.apikey
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+    
+    try:
+      output = fn.dataRequest(linkAPI, output_type)
+      return output
+    except ValueError:
+      raise WebRequestError ('Something went wrong.')  
+    
+    
+
+
+def getMarketsBySymbol(symbols, output_type=None):
+    """
+    Returns a markets information for specific symbols.
+    ==========================================================
+    Parameters:
+    -----------
+    symbols: string or list.
+            String to get data for symbol. List of strings to get data for
+             several symbols. For example, symbols = ['aapl:us', 'indu:ind'].
+             
+    output_type: string.
+             'dict'(default), 'df' for data frame,
+             'raw' for list of unparsed data. 
+    Example
+    -------
+    getMarketsBySymbol(symbols = 'indu:ind')
+    getMarketsBySymbol(symbols = ['aapl:us', 'indu:ind'], output_type = 'raw')
+    """
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+
+    if type(symbols) is not str:        
+        linkAPI = 'https://api.tradingeconomics.com/markets/symbol/' + quote(",".join(symbols), safe='') 
+    else:   
+        linkAPI = 'https://api.tradingeconomics.com/markets/symbol/' + quote(symbols, safe='')
+    
+    try:
+        linkAPI += '?c=' + glob.apikey
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+    
+    try:
+      output = fn.dataRequest(linkAPI, output_type)
+      return output
+    except ValueError:
+      raise WebRequestError ('Something went wrong.')  
+
+
+def getMarketsIntraday(symbols, initDate=None, endDate=None, output_type=None):
+    """
+    Returns a markets intraday information for specific symbols.
+    ==========================================================
+    Parameters:
+    -----------
+    symbols: string or list.
+            String to get data for symbol. List of strings to get data for
+             several symbols. For example, symbols = ['aapl:us', 'indu:ind'].
+    
+    initDate: string with format: YYYY-MM-DD.
+             For example: '2011-01-01' 
+    endDate: string with format: YYYY-MM-DD.    
+    output_type: string.
+             'dict'(default), 'df' for data frame,
+             'raw' for list of unparsed data. 
+    Example
+    -------
+    getMarketsIntraday(symbols = 'indu:ind')
+    getMarketsIntraday(symbols = 'indu:ind', initDate='2018-03-13 15:30')
+    getMarketsIntraday(symbols = ['aapl:us', 'indu:ind'], initDate='2022-01-01', endDate='2022-12-31', output_type = 'raw')
+    """
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+
+    if type(symbols) is not str:        
+        linkAPI = 'https://api.tradingeconomics.com/markets/intraday/' + quote(",".join(symbols), safe='') 
+    else:   
+        linkAPI = 'https://api.tradingeconomics.com/markets/intraday/' + quote(symbols, safe='')
+    
+    try:
+        linkAPI += '?c=' + glob.apikey
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+    
+    linkAPI = fn.checkDates(linkAPI, initDate, endDate)
+
+    try:
+      output = fn.dataRequest(linkAPI, output_type)
+      return output
+    except ValueError:
+      raise WebRequestError ('Something went wrong.')  
+
+def getMarketsPeers(symbols, output_type = None):
+    """
+    Returns a markets peers information for specific symbols.
+    ==========================================================
+    Parameters:
+    -----------
+    symbols: string or list.
+            String to get data for symbol. List of strings to get data for
+             several symbols. For example, symbols = ['aapl:us', 'indu:ind'].
+             
+    output_type: string.
+             'dict'(default), 'df' for data frame,
+             'raw' for list of unparsed data. 
+    Example
+    -------
+    getMarketsPeers(symbols = 'indu:ind')
+    getMarketsPeers(symbols = ['aapl:us', 'indu:ind'], output_type = 'raw')
+    """
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+
+    if type(symbols) is not str:        
+        linkAPI = 'https://api.tradingeconomics.com/markets/peers/' + quote(",".join(symbols), safe='') 
+    else:   
+        linkAPI = 'https://api.tradingeconomics.com/markets/peers/' + quote(symbols, safe='')
+    
+    try:
+        linkAPI += '?c=' + glob.apikey
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+    try:
+      output = fn.dataRequest(linkAPI, output_type)
+      return output
+    except ValueError:
+      raise WebRequestError ('Something went wrong.')  
+
+def getMarketsComponents(symbols, output_type = None):
+    """
+    Returns a stock market index components information for specific symbols.
+    ==========================================================
+    Parameters:
+    -----------
+    symbols: string or list.
+            String to get data for symbol. List of strings to get data for
+             several symbols. For example, symbols = ['aapl:us', 'indu:ind'].
+             
+    output_type: string.
+             'dict'(default), 'df' for data frame,
+             'raw' for list of unparsed data. 
+    Example
+    -------
+    getMarketsComponents(symbols = 'psi20:ind')
+    getMarketsComponents(symbols = ['psi20:ind', 'indu:ind'], output_type = 'raw')
+    """
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+
+    if type(symbols) is not str:        
+        linkAPI = 'https://api.tradingeconomics.com/markets/components/' + quote(",".join(symbols), safe='') 
+    else:   
+        linkAPI = 'https://api.tradingeconomics.com/markets/components/' + quote(symbols, safe='')
+    
+    try:
+        linkAPI += '?c=' + glob.apikey
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+    try:
+      output = fn.dataRequest(linkAPI, output_type)
+      return output
+    except ValueError:
+      raise WebRequestError ('Something went wrong.')  
+
+def getMarketsSearch(country=None, category = None, page = None, output_type = None):    
+    """
+    Search for country, category and page number.
+    ==========================================================
+    Parameters:
+    -----------
+    symbols: string.
+            String to get data for country and category. 
+    
+    output_type: string.
+             'dict'(default), 'df' for data frame,
+             'raw' for list of unparsed data. 
+    Example
+    -------
+    getMarketsSearch(country = 'japan', category = None, page = None, output_type = None)
+    getMarketsSearch(country = 'japan', category = 'index', page = None, output_type = None)
+    getMarketsSearch(country = 'japan', category = ['index', 'markets'], page = None, output_type = None)
+    getMarketsSearch(country = 'japan', category = 'index', page = None, output_type = None)
+    """
+    
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+
+    if type(country) is not str:        
+        linkAPI = 'https://api.tradingeconomics.com/markets/search/' + quote(",".join(country), safe='') 
+    else:   
+        linkAPI = 'https://api.tradingeconomics.com/markets/search/' + quote(country, safe='')
+    if (category) is not None:    
+        linkAPI = checkCategory(linkAPI, category)       
+    if (page) is not None:
+        linkAPI = checkPage(linkAPI, page)
+    
+    try:
+        if (category)is not None:
+            linkAPI += '&c=' + glob.apikey
+        else:
+            linkAPI += '?c=' + glob.apikey
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+    
+    try:
+      output = fn.dataRequest(linkAPI, output_type)
+      return output
+    except ValueError:
+      raise WebRequestError ('Something went wrong.')  
+
+
+def getMarketsForecasts(category=None, symbol=None,  output_type = None):
+    """
+    Returns a stock market forecast information for specific symbols and categories.
+    ================================================================================
+    Parameters:
+    -----------
+    symbol: string or list.
+            String to get data for symbol. List of strings to get data for
+             several symbols. For example, symbols = ['aapl:us', 'indu:ind'].
+    category: string.
+            String to get data by category.  
+            For example, category = 'index'         
+             
+    output_type: string.
+             'dict'(default), 'df' for data frame,
+             'raw' for list of unparsed data. 
+    Example
+    -------
+    getMarketsForecasts(category = 'bond')
+    getMarketsForecasts(symbol = ['psi20:ind', 'indu:ind'], output_type = 'df')
+    getMarketsForecasts(symbol =  'indu:ind', output_type = 'df')
+    """
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context    
+  
+    if type(symbol) is list: 
+        linkAPI = 'http://api.tradingeconomics.com/markets/forecasts' + '/symbol/' + quote(",".join(symbol), safe='') 
+             
+    else:  
+       linkAPI = 'http://api.tradingeconomics.com/markets/forecasts' + '/symbol/' + quote(str(symbol)) 
+    
+    if category is not None:
+        linkAPI = 'http://api.tradingeconomics.com/markets/forecasts/' + quote(category)
+       
+
+    try:
+        linkAPI += '?c=' + glob.apikey
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+    
+    try:
+    #   output = fn.makeRequestAndParse(linkAPI, output_type)
+      output = fn.dataRequest(linkAPI, output_type)
+      return output
+    except ValueError:
+      raise WebRequestError ('Something went wrong.')   
+
+
+def getMarketsIntradayByInterval(symbol, interval, initDate,endDate,output_type=None):
+    """
+    Returns Aggregate intraday prices by interval - allowed intervals: 1m, 5m, 10m, 15m, 30m, 1h, 2h, 4h.
+    =================================================================================
+    Parameters:
+    -----------
+        symbol: string.
+                symbol = 'CL1:COM'
+                symbol = ['CL1:COM','AAPL:US']
+        interval: string
+                interval='1m'
+        initDate: string.
+                initDate = '2021-01-01'
+        endDate:string.
+                endDate = '2021-01-10'
+        
+        output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+    Notes
+    -----
+    
+    
+    Example
+    -------
+            getMarketsIntradayByInterval(symbol='CL1:COM',interval='1m',initDate='2022-01-01',endDate='2023-12-01',output_type='df')
+            getMarketsIntradayByInterval(symbol=['CL1:COM','AAPL:US'],interval='1m',initDate='2022-01-01',endDate='2022-12-01',output_type='df')
+    """
+            
+    
+    # d is a dictionary used for create the api url
+    d = {
+        'url_base': 'https://api.tradingeconomics.com/markets/intraday',
+        'symbol': f'/{fn.stringOrList(symbol)}',
+        'interval' : f'?agr={fn.stringOrList(interval)}',
+        'init_date': '',
+        'end_date':'',
+        'key': f'&client={glob.apikey}',
+        'output_type' : ''
+    }
+    if initDate and endDate :     
+
+        fn.validate(initDate)
+        fn.validate(endDate)
+        fn.validatePeriod(initDate, endDate)
+        # #it will parse endDate when initDate and endData are the same. 
+        # endDate = (lambda x, y : f"{endDate[0:8]}{(int(endDate[8:])+1)}" if x==y else endDate)(initDate,endDate)
+        # d['init_date']=f'&d1={initDate}'
+        # d['end_date']=f'&d2={endDate}'
+
+    
+
+    api_url_request = "%s%s%s%s%s%s" % (d['url_base'], d['symbol'], d['interval'],  d['init_date'],  d['end_date'],  d['key']) 
+
+    try:
+      # print(api_url_request)
+      output = fn.dataRequest(api_url_request, output_type)
+      return output
+    except ValueError:
+      raise WebRequestError ('Something went wrong.')   
+    
+
+
+def getMarketsStockDescriptions(symbol = None,country = None, output_type=None):
+    """
+    Returns Markets Descriptions
+    =================================================================================
+    Parameters:
+    -----------
+        symbol: string or list.
+                symbol = 'AAPL:US'
+                symbol = ['AAPL:US','FB:US']
+        
+        country: string or list
+                country = 'france'
+                countr = ['france','portugal']
+        
+        
+        output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+    Notes
+    -----
+    
+    
+    Example
+    -------
+            getMarketsStockDescriptions(symbol='AAPL:US',output_type='df')
+            getMarketsStockDescriptions(symbol=['AAPL:US','FB:US'],output_type='df')
+            getMarketsStockDescriptions(country='france',output_type='df')
+            getMarketsStockDescriptions(country=['france','portugal'],output_type='df')
+    """
+            
+    # url example: 'https://api.tradingeconomics.com/markets/stockdescriptions/symbol/aapl:us,fb:us?c=guest:guest'
+    # https://api.tradingeconomics.com/markets/stockdescriptions/country/france,portugal?c=guest:guest
+
+    # d is a dictionary used for create the api url
+    d = {
+        'url_base': 'https://api.tradingeconomics.com/markets/stockdescriptions',
+        'symbol': '',
+        'country': '',
+        'key': f'?c={glob.apikey}',
+        'output_type' : ''
+    }
+
+    if symbol:
+        d['symbol'] = f'/symbol/{(fn.stringOrList(symbol))}'
+    
+    if country:
+        d['country'] = f'/country/{(fn.stringOrList(country))}'
+
+    if country and symbol or country is None and symbol is None:
+        return 'You have to pass country or symbol'
+    
+    
+
+    api_url_request = "%s%s%s%s" % (d['url_base'], d['symbol'],d['country'],  d['key']) 
+    try:
+      output = fn.dataRequest(api_url_request, output_type)
+      return output
+    except ValueError:
+      raise WebRequestError ('Something went wrong.')   
+
+def getMarketsSymbology(symbol = None,ticker = None, isin=None, country=None ,output_type=None):
+    """
+    Returns Markets Descriptions
+    =================================================================================
+    Parameters:
+    -----------
+        symbol: string 
+                symbol = 'AAPL:US'
+                
+        ticker: string 
+                ticker = 'aapl'
+        
+        isin: string 
+                isin = 'US0378331005'
+
+        country: string 
+                country = 'United States'                
+        
+        
+        output_type: string.
+            'dict'(default) for dictionary format output, 'df' for data frame,
+            'raw' for list of dictionaries directly from the web. 
+    Notes
+    -----
+    
+    
+    Example
+    -------
+            getMarketsSymbology(symbol='AAPL:US',output_type='df')
+            getMarketsSymbology(ticker='aapl',output_type='df')
+            getMarketsSymbology(isin='US0378331005',output_type='df')
+            getMarketsSymbology(country='United States',output_type='df')
+            
+    """
+    #validateParameters
+    parametersList = []
+    (lambda x : parametersList.append(x) if x != None else None )(symbol) 
+    (lambda x : parametersList.append(x) if x != None else None )(ticker) 
+    (lambda x : parametersList.append(x) if x != None else None )(isin) 
+    (lambda x : parametersList.append(x) if x != None else None )(country)
+
+    if len(parametersList) > 1:
+      print('Only one argument must be provided for each request')
+      return 
+          
+
+    # d is a dictionary used for create the api url
+    d = {
+        'url_base': 'https://api.tradingeconomics.com/markets/symbology',
+        'symbol': '',
+        'ticker': '',
+        'isin': '',
+        'country': '',
+        'key': f'?c={glob.apikey}',
+        'output_type' : ''
+    }
+
+
+    if symbol:
+        d['symbol'] = f'/symbol/{(fn.stringOrList(symbol))}'
+    
+    if ticker:
+        d['ticker'] = f'/ticker/{(fn.stringOrList(ticker))}'
+    
+    if isin:
+        d['isin'] = f'/isin/{(fn.stringOrList(isin))}'
+
+    if country:
+        d['country'] = f'/country/{(fn.stringOrList(country))}'
+
+    api_url_request = "%s%s%s%s%s%s" % (d['url_base'], d['symbol'],d['ticker'],  d['isin'],d['country'],d['key']) 
+    try:
+      output = fn.dataRequest(api_url_request, output_type)
+      return output
+    except ValueError:
+      raise WebRequestError ('Something went wrong.')   
+
+def getStocksByCountry (country:str,output_type=None):
+    """
+    Returns Stocks List to a specific country
+    =================================================================================
+    Parameters:
+    -----------
+        country: string 
+                symbol = 'United States'
+                
+        output_type: string.
+            'dict'(default) for dictionary format output, 'df' for data frame,
+            'raw' for list of dictionaries directly from the web. 
+    Notes
+    -----
+    
+    
+    Example
+    -------
+            getStocksByCountry(country='United States',output_type='df')
+            
+    """
+    
+          
+
+    # d is a dictionary used for create the api url
+    d = {
+        'url_base': 'https://api.tradingeconomics.com/markets/country/',
+        'country': '',
+        'key': f'?c={glob.apikey}',
+        'output_type' : ''
+    }
+
+    try:
+        if type(country) == str:
+            d['country'] = f'{quote(country)}'
+        else:
+          raise AttributeError ('country must be a string')
+    except Exception as e:
+      raise e
+    
+    
+
+    api_url_request = "%s%s%s" % (d['url_base'], d['country'],d['key']) 
+    try:
+      output = fn.dataRequest(api_url_request, output_type)
+      return output
+    except ValueError:
       raise WebRequestError ('Something went wrong.')
```

### Comparing `tradingeconomics-4.2.8/tradingeconomics/news.py` & `tradingeconomics-4.2.9/tradingeconomics/news.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,389 +1,389 @@
-import json
-import itertools
-import urllib 
-import pandas as pd
-import sys
-from datetime import *
-from dateutil.relativedelta import relativedelta
-from . import functions as fn
-from . import glob
-import ssl
-
-PY3 = sys.version_info[0] == 3
-
-if PY3: # Python 3+
-    from urllib.request import urlopen
-    from urllib.parse import quote
-else: # Python 2.X
-    from urllib import urlopen
-    from urllib import quote
-
-class ParametersError(ValueError):
-    pass
-
-class DateError(ValueError):
-    pass
-
-class CredentialsError(ValueError):
-    pass
-
-class LoginError(AttributeError):
-    pass
-
-class WebRequestError(ValueError):
-    pass
-
-def checkIndex(linkAPI, start):
-    if start != None:
-        linkAPI += '&start={0}'.format(start)  
-    return linkAPI
-
-def checkLimit(linkAPI, limit):
-    if limit != None:
-        linkAPI += '&limit={0}'.format(limit)
-    return linkAPI
-
-
-def checkNewsIndic(indicator): 
-    linkAPI = 'https://api.tradingeconomics.com/news/indicator/'      
-    if type(indicator) is str:
-        linkAPI += '/' + quote(indicator, safe="")
-    else:
-        linkAPI += '/' + quote(",".join(indicator), safe="")
-    return linkAPI
-
-def checkNewsCountry(country):
-    linkAPI = 'https://api.tradingeconomics.com/news/country/'      
-    if type(country) is str:
-        linkAPI +=  '/' + quote(country, safe="")
-    else:
-        linkAPI += '/' + quote(",".join(country), safe="")
-    return linkAPI
-
-def getNewsLink(country, indicator):
-    linkAPI = 'https://api.tradingeconomics.com/news/country/'    
-    if type(country) is str:
-        linkAPI += quote(country, safe="")
-    else: 
-        linkAPI += quote(",".join(country), safe="") 
-    if type(indicator) is str:
-        linkAPI += '/' + quote(indicator, safe="")
-    else: 
-        linkAPI += '/' + quote(",".join(indicator), safe="") 
-    return linkAPI
-  
-def getNewsResults(webResults, country):
-        names = ['id', 'title', 'date', 'description', 'country', 'category', 'symbol', 'url']
-        names2 = ['id', 'title', 'date', 'description', 'country', 'category', 'symbol', 'url']
-        maindf = pd.DataFrame()  
-        for i in range(len(names)):
-            names[i] = [d[names2[i]]  for d in webResults]
-            maindf = pd.concat([maindf, pd.DataFrame(names[i], columns = [names2[i]])], axis = 1) 
-            maindf['country'] =  maindf['country'].map(lambda x: x.strip())
-
-
-def checkArticleLink (country, indicator):
-    linkAPI = 'https://api.tradingeconomics.com/articles/country/'    
-    if type(country) is str:
-        linkAPI += quote(country)
-    else: 
-        linkAPI += quote(",".join(country), safe="") 
-    if type(indicator) is str:
-        linkAPI += '/' + quote(indicator, safe="")
-    else: 
-        linkAPI += '/' + quote(",".join(indicator), safe="") 
-    return linkAPI
-
-def checkArticleCountry(country):
-    linkAPI = 'https://api.tradingeconomics.com/articles/country'      
-    if country != None:
-        if type(country) == str:
-            linkAPI += '/' + quote(country, safe="")
-        else:    
-            linkAPI += '/' + quote(",".join(country), safe="")
-     
-    return linkAPI
-
-def checkArticleIndic(indicator): 
-    linkAPI = 'https://api.tradingeconomics.com/articles/indicator/'      
-    if indicator != None:
-        if type(indicator) == str:
-            linkAPI += '/' + indicator
-        else:    
-            linkAPI += '/' + quote(",".join(indicator), safe="")
-
-    return linkAPI
-
-def checkArticleLimit(linkAPI, lim):
-    if lim != None:
-        linkAPI += '&lim={0}'.format(lim)
-    return linkAPI
-
-def getArticleResults(webResults, id):
-        names = ['id', 'title', 'date', 'description', 'content', 'country', 'category', 'symbol', 'url']
-        names2 = ['id', 'title', 'date', 'description', 'content', 'country', 'category', 'symbol', 'url']
-        maindf = pd.DataFrame()  
-        for i in range(len(names)):
-            names[i] = [d[names2[i]]  for d in webResults]
-            maindf = pd.concat([maindf, pd.DataFrame(names[i], columns = [names2[i]])], axis = 1) 
-            maindf['category'] =  maindf['category'].map(lambda x: x.strip())
-
-def checkArticleId(id):
-    linkAPI = 'https://api.tradingeconomics.com/articles/id/'      
-    if type(id) is str:
-        linkAPI +=  '/' + quote(str(id))
-    else:
-        linkAPI += '/' + quote(",".join(str(id)))
-    return linkAPI
-
-
-
-
-
-
-def getArticles(country = None, indicator = None, initDate = None, endDate = None, start = None, lim = None, output_type = None):
-    """
-    Return a list of all articles, article by indicators by country with date interval, and list by limit or start index.
-    =================================================================================
-
-    Parameters:
-    -----------
-    country: string or list.
-            List of strings for one country or several countries, for example: 
-            country = ['country_name', 'country_name']
-            country = 'country_name'
-            List of strings for several countries and indicators or one country and one indicator, for example: 
-            country = ['country_name', 'country_name'], indicator = ['inflation rate', 'interest rate']
-            country = 'country_name', indicator = 'inflation rate'
-            list of strings for one or more countries with date interval, example: 
-            country = 'country_name', initDate = '2015-10-10', endDate = '2017-10-10' 
-            country = ['country_name', 'country_name], initDate = '2015-10-10', endDate = '2017-10-10'
-    indicators: string or list.
-            List of strings for several indicators or one indicator, for example: 
-            indicator = 'indicator_name'  
-            indicator = ['indicator_name', 'indicator_name']
-    start and lim: string or list.
-            articles list by start index and/or by limit for example:
-            country = 'country_name', start = 20, lim = 100
-            indicator = 'indicator_name', start = 20, lim = 100
-            country = 'country_name', indicator = 'indicator_name', start = 20, lim = 100            
-    initDate: string with format: YYYY-MM-DD.
-            For example: '2011-01-01' 
-    endDate: string with format: YYYY-MM-DD.            
-    output_type: string.
-            'dict'(default) for dictionary format output, 'df' for data frame,
-            'raw' for list of dictionaries directly from the web. 
-
-    Notes
-    -----
-     Without parameters a list of articles will be provided. 
-
-    Example
-    -------
-    getArticles(country = ['United States', 'Portugal'], indicator = ['Imports','Interest rate'])
-
-    getArticles( start = 10, lim = 20, output_type = 'df')
-
-    getArticles(country = 'United States''2015-10-10', endDate = '2017-10-10')
-
-    """          
-
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-
-    if country != None and indicator != None:
-        linkAPI = checkArticleLink(country, indicator) 
-    elif country != None and indicator == None:
-        linkAPI = checkArticleCountry(country)      
-    elif country == None and indicator != None:
-        linkAPI = checkArticleIndic(indicator)
-    else:
-        linkAPI = 'https://api.tradingeconomics.com/articles/'
-    
-    if (initDate != None) and (endDate != None) :
-        try: 
-            fn.validate(initDate)
-        except ValueError:
-            raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
-        try: 
-            fn.validate(endDate)
-        except ValueError:
-            raise DateError ('Incorrect endDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
-        try:        
-            fn.validatePeriod(initDate, endDate)
-        except ValueError:
-            raise DateError ('Invalid time period.')
-        linkAPI += '/from' + '/' + initDate + '/' + endDate
-    
-    elif (initDate != None) and endDate == None :        
-        try: 
-            fn.validate(initDate)
-        except ValueError:
-            raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
-            if initDate > str(date.today()):
-                raise DateError ('Initial date out of range.')
-        linkAPI += '/from' + initDate
-    
-    elif initDate == None and (endDate != None):
-        initDate = (datetime.str(endDate, '%Y-%m-%d') - relativedelta(months=6)).strftime('%Y-%m-%d')
-        linkAPI += '/from' + '/' + initDate + '/' + endDate 
-     
-    try:
-        linkAPI += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-    
-    linkAPI = checkArticleLimit(linkAPI, lim)
-    linkAPI = checkIndex(linkAPI, start)
-
-    try:
-        print(linkAPI)
-        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
-    except Exception as e:
-        print(e)         
-
-def getArticleId(id = None, output_type = None):
-    """
-    Return one id of an article.
-    =================================================================================
-
-    Parameters:
-    -----------
-    id: string.
-            Information of one article searched by it's identifier.
-    output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web. 
-
-    Notes
-    -----
-    To get results it must have a given id. 
-
-    Example
-    -------
-    getArticleId(id = '20580', output_type = None)
-    
-    """ 
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-    if type(id) !=None:        
-        linkAPI =  checkArticleId(id)
-            
-    try:
-        linkAPI += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-
-    try:
-        print(linkAPI)
-        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
-    except Exception as e:
-        print(e) 
-
-def getNews(country = None,  indicator = None, start= None, limit = None, output_type = None, start_date=None, end_date=None):
-    """
-    Return a list of all news, indicators by country, limit and start index or start_date
-    and end_date.
-    =================================================================================
-
-    Parameters:
-    -----------
-    country: string or list.
-             String for one country information. List of strings for 
-             several countrys, for example country = ['country_name', 'country_name'].
-    indicators: string or list.
-             String for one indicator. List of strings for several indicators, for example 
-             indicators = 'indicator_name' or 
-             indicators = ['indicator_name', 'indicator_name']
-    start: string.
-            start = '15'
-    limit: string
-            limit = '10'
-    start_date: string.
-            start_date = '2021-02-03'
-    end_date: string.
-            end_date = '2021-07-03'
-
-    output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web. 
-
-    Notes
-    -----
-    All parameters are optional. Without parameters a list of all news will be provided. 
-
-    Example
-    -------
-    getNews(output_type='df')
-    
-    getNews(start_date='2021-02-02', end_date='2021-03-03')
-
-    getNews(start='15', limit='15', output_type='df')
-
-    getNews(indicator='inflation rate', start_date='2021-02-02', end_date='2021-03-03')
-
-    getNews(indicator=['inflation rate', 'gdp'])
-
-    getNews(indicator=['Commodity', 'Stock Market'])
-
-    getNews(country=['brazil','canada'], indicator=['Housing Starts', 'Stock Market'], start_date='2021-02-02', end_date='2021-03-03')
-
-    getNews(country = 'United States', indicator = 'Imports', start = 10, limit = 20, output_type = 'df')
-
-    getNews(country = ['United States', 'Portugal'], indicator = ['Imports','Exports'])
-    
-    getNews(country=['brazil','canada'])
-    """  
-    
-    d = {
-        'url_base': 'https://api.tradingeconomics.com/news',
-        'indicator': '',
-        'country': '',
-        'start':'',
-        'limit':'',
-        'start_date':'',
-        'end_date':'',
-
-        'key': f'?c={glob.apikey}',
-        'output_type' : ''
-    }
-
-    if start and start_date:
-        return 'Please, enter the pair "start" and "limit" or the pair "start_date" and "end_date"'
-
-    if start and limit:
-        d['start'] = f'&start={start}'
-        
-        d['limit'] = f'&limit={limit}'
-        
-    
-        
-    if start_date and end_date and not start and not limit:
-        d['start_date'] = f'&d1={fn.checkDates(start_date)}'
-        d['end_date'] = f'&d2={fn.checkDates(end_date)}'
-
-    if indicator:
-        d['indicator'] = f'/indicator/{(fn.stringOrList(indicator))}'
-    
-    if country:
-        d['country'] = f'/country/{(fn.stringOrList(country))}'
-
-    if country and indicator:
-        d['indicator'] = f'/{fn.stringOrList(indicator)}'
-
-
-    api_url_request = "%s%s%s%s%s%s%s%s" % (d['url_base'], d['country'],d['indicator'], d['key'],d['limit'],d['start'],d['start_date'],d['end_date']) 
-    # print(api_url_request)
-    return fn.dataRequest(api_request=api_url_request, output_type=output_type)
-
-
-
-
+import json
+import itertools
+import urllib 
+import pandas as pd
+import sys
+from datetime import *
+from dateutil.relativedelta import relativedelta
+from . import functions as fn
+from . import glob
+import ssl
+
+PY3 = sys.version_info[0] == 3
+
+if PY3: # Python 3+
+    from urllib.request import urlopen
+    from urllib.parse import quote
+else: # Python 2.X
+    from urllib import urlopen
+    from urllib import quote
+
+class ParametersError(ValueError):
+    pass
+
+class DateError(ValueError):
+    pass
+
+class CredentialsError(ValueError):
+    pass
+
+class LoginError(AttributeError):
+    pass
+
+class WebRequestError(ValueError):
+    pass
+
+def checkIndex(linkAPI, start):
+    if start != None:
+        linkAPI += '&start={0}'.format(start)  
+    return linkAPI
+
+def checkLimit(linkAPI, limit):
+    if limit != None:
+        linkAPI += '&limit={0}'.format(limit)
+    return linkAPI
+
+
+def checkNewsIndic(indicator): 
+    linkAPI = 'https://api.tradingeconomics.com/news/indicator/'      
+    if type(indicator) is str:
+        linkAPI += '/' + quote(indicator, safe="")
+    else:
+        linkAPI += '/' + quote(",".join(indicator), safe="")
+    return linkAPI
+
+def checkNewsCountry(country):
+    linkAPI = 'https://api.tradingeconomics.com/news/country/'      
+    if type(country) is str:
+        linkAPI +=  '/' + quote(country, safe="")
+    else:
+        linkAPI += '/' + quote(",".join(country), safe="")
+    return linkAPI
+
+def getNewsLink(country, indicator):
+    linkAPI = 'https://api.tradingeconomics.com/news/country/'    
+    if type(country) is str:
+        linkAPI += quote(country, safe="")
+    else: 
+        linkAPI += quote(",".join(country), safe="") 
+    if type(indicator) is str:
+        linkAPI += '/' + quote(indicator, safe="")
+    else: 
+        linkAPI += '/' + quote(",".join(indicator), safe="") 
+    return linkAPI
+  
+def getNewsResults(webResults, country):
+        names = ['id', 'title', 'date', 'description', 'country', 'category', 'symbol', 'url']
+        names2 = ['id', 'title', 'date', 'description', 'country', 'category', 'symbol', 'url']
+        maindf = pd.DataFrame()  
+        for i in range(len(names)):
+            names[i] = [d[names2[i]]  for d in webResults]
+            maindf = pd.concat([maindf, pd.DataFrame(names[i], columns = [names2[i]])], axis = 1) 
+            maindf['country'] =  maindf['country'].map(lambda x: x.strip())
+
+
+def checkArticleLink (country, indicator):
+    linkAPI = 'https://api.tradingeconomics.com/articles/country/'    
+    if type(country) is str:
+        linkAPI += quote(country)
+    else: 
+        linkAPI += quote(",".join(country), safe="") 
+    if type(indicator) is str:
+        linkAPI += '/' + quote(indicator, safe="")
+    else: 
+        linkAPI += '/' + quote(",".join(indicator), safe="") 
+    return linkAPI
+
+def checkArticleCountry(country):
+    linkAPI = 'https://api.tradingeconomics.com/articles/country'      
+    if country != None:
+        if type(country) == str:
+            linkAPI += '/' + quote(country, safe="")
+        else:    
+            linkAPI += '/' + quote(",".join(country), safe="")
+     
+    return linkAPI
+
+def checkArticleIndic(indicator): 
+    linkAPI = 'https://api.tradingeconomics.com/articles/indicator/'      
+    if indicator != None:
+        if type(indicator) == str:
+            linkAPI += '/' + indicator
+        else:    
+            linkAPI += '/' + quote(",".join(indicator), safe="")
+
+    return linkAPI
+
+def checkArticleLimit(linkAPI, lim):
+    if lim != None:
+        linkAPI += '&lim={0}'.format(lim)
+    return linkAPI
+
+def getArticleResults(webResults, id):
+        names = ['id', 'title', 'date', 'description', 'content', 'country', 'category', 'symbol', 'url']
+        names2 = ['id', 'title', 'date', 'description', 'content', 'country', 'category', 'symbol', 'url']
+        maindf = pd.DataFrame()  
+        for i in range(len(names)):
+            names[i] = [d[names2[i]]  for d in webResults]
+            maindf = pd.concat([maindf, pd.DataFrame(names[i], columns = [names2[i]])], axis = 1) 
+            maindf['category'] =  maindf['category'].map(lambda x: x.strip())
+
+def checkArticleId(id):
+    linkAPI = 'https://api.tradingeconomics.com/articles/id/'      
+    if type(id) is str:
+        linkAPI +=  '/' + quote(str(id))
+    else:
+        linkAPI += '/' + quote(",".join(str(id)))
+    return linkAPI
+
+
+
+
+
+
+def getArticles(country = None, indicator = None, initDate = None, endDate = None, start = None, lim = None, output_type = None):
+    """
+    Return a list of all articles, article by indicators by country with date interval, and list by limit or start index.
+    =================================================================================
+
+    Parameters:
+    -----------
+    country: string or list.
+            List of strings for one country or several countries, for example: 
+            country = ['country_name', 'country_name']
+            country = 'country_name'
+            List of strings for several countries and indicators or one country and one indicator, for example: 
+            country = ['country_name', 'country_name'], indicator = ['inflation rate', 'interest rate']
+            country = 'country_name', indicator = 'inflation rate'
+            list of strings for one or more countries with date interval, example: 
+            country = 'country_name', initDate = '2015-10-10', endDate = '2017-10-10' 
+            country = ['country_name', 'country_name], initDate = '2015-10-10', endDate = '2017-10-10'
+    indicators: string or list.
+            List of strings for several indicators or one indicator, for example: 
+            indicator = 'indicator_name'  
+            indicator = ['indicator_name', 'indicator_name']
+    start and lim: string or list.
+            articles list by start index and/or by limit for example:
+            country = 'country_name', start = 20, lim = 100
+            indicator = 'indicator_name', start = 20, lim = 100
+            country = 'country_name', indicator = 'indicator_name', start = 20, lim = 100            
+    initDate: string with format: YYYY-MM-DD.
+            For example: '2011-01-01' 
+    endDate: string with format: YYYY-MM-DD.            
+    output_type: string.
+            'dict'(default) for dictionary format output, 'df' for data frame,
+            'raw' for list of dictionaries directly from the web. 
+
+    Notes
+    -----
+     Without parameters a list of articles will be provided. 
+
+    Example
+    -------
+    getArticles(country = ['United States', 'Portugal'], indicator = ['Imports','Interest rate'])
+
+    getArticles( start = 10, lim = 20, output_type = 'df')
+
+    getArticles(country = 'United States''2015-10-10', endDate = '2017-10-10')
+
+    """          
+
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+
+    if country != None and indicator != None:
+        linkAPI = checkArticleLink(country, indicator) 
+    elif country != None and indicator == None:
+        linkAPI = checkArticleCountry(country)      
+    elif country == None and indicator != None:
+        linkAPI = checkArticleIndic(indicator)
+    else:
+        linkAPI = 'https://api.tradingeconomics.com/articles/'
+    
+    if (initDate != None) and (endDate != None) :
+        try: 
+            fn.validate(initDate)
+        except ValueError:
+            raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
+        try: 
+            fn.validate(endDate)
+        except ValueError:
+            raise DateError ('Incorrect endDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
+        try:        
+            fn.validatePeriod(initDate, endDate)
+        except ValueError:
+            raise DateError ('Invalid time period.')
+        linkAPI += '/from' + '/' + initDate + '/' + endDate
+    
+    elif (initDate != None) and endDate == None :        
+        try: 
+            fn.validate(initDate)
+        except ValueError:
+            raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
+            if initDate > str(date.today()):
+                raise DateError ('Initial date out of range.')
+        linkAPI += '/from' + initDate
+    
+    elif initDate == None and (endDate != None):
+        initDate = (datetime.str(endDate, '%Y-%m-%d') - relativedelta(months=6)).strftime('%Y-%m-%d')
+        linkAPI += '/from' + '/' + initDate + '/' + endDate 
+     
+    try:
+        linkAPI += '?c=' + glob.apikey
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+    
+    linkAPI = checkArticleLimit(linkAPI, lim)
+    linkAPI = checkIndex(linkAPI, start)
+
+    try:
+        print(linkAPI)
+        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
+    except Exception as e:
+        print(e)         
+
+def getArticleId(id = None, output_type = None):
+    """
+    Return one id of an article.
+    =================================================================================
+
+    Parameters:
+    -----------
+    id: string.
+            Information of one article searched by it's identifier.
+    output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+
+    Notes
+    -----
+    To get results it must have a given id. 
+
+    Example
+    -------
+    getArticleId(id = '20580', output_type = None)
+    
+    """ 
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+    if type(id) !=None:        
+        linkAPI =  checkArticleId(id)
+            
+    try:
+        linkAPI += '?c=' + glob.apikey
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+
+    try:
+        print(linkAPI)
+        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
+    except Exception as e:
+        print(e) 
+
+def getNews(country = None,  indicator = None, start= None, limit = None, output_type = None, start_date=None, end_date=None):
+    """
+    Return a list of all news, indicators by country, limit and start index or start_date
+    and end_date.
+    =================================================================================
+
+    Parameters:
+    -----------
+    country: string or list.
+             String for one country information. List of strings for 
+             several countrys, for example country = ['country_name', 'country_name'].
+    indicators: string or list.
+             String for one indicator. List of strings for several indicators, for example 
+             indicators = 'indicator_name' or 
+             indicators = ['indicator_name', 'indicator_name']
+    start: string.
+            start = '15'
+    limit: string
+            limit = '10'
+    start_date: string.
+            start_date = '2021-02-03'
+    end_date: string.
+            end_date = '2021-07-03'
+
+    output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+
+    Notes
+    -----
+    All parameters are optional. Without parameters a list of all news will be provided. 
+
+    Example
+    -------
+    getNews(output_type='df')
+    
+    getNews(start_date='2021-02-02', end_date='2021-03-03')
+
+    getNews(start='15', limit='15', output_type='df')
+
+    getNews(indicator='inflation rate', start_date='2021-02-02', end_date='2021-03-03')
+
+    getNews(indicator=['inflation rate', 'gdp'])
+
+    getNews(indicator=['Commodity', 'Stock Market'])
+
+    getNews(country=['brazil','canada'], indicator=['Housing Starts', 'Stock Market'], start_date='2021-02-02', end_date='2021-03-03')
+
+    getNews(country = 'United States', indicator = 'Imports', start = 10, limit = 20, output_type = 'df')
+
+    getNews(country = ['United States', 'Portugal'], indicator = ['Imports','Exports'])
+    
+    getNews(country=['brazil','canada'])
+    """  
+    
+    d = {
+        'url_base': 'https://api.tradingeconomics.com/news',
+        'indicator': '',
+        'country': '',
+        'start':'',
+        'limit':'',
+        'start_date':'',
+        'end_date':'',
+
+        'key': f'?c={glob.apikey}',
+        'output_type' : ''
+    }
+
+    if start and start_date:
+        return 'Please, enter the pair "start" and "limit" or the pair "start_date" and "end_date"'
+
+    if start and limit:
+        d['start'] = f'&start={start}'
+        
+        d['limit'] = f'&limit={limit}'
+        
+    
+        
+    if start_date and end_date and not start and not limit:
+        d['start_date'] = f'&d1={fn.checkDates(start_date)}'
+        d['end_date'] = f'&d2={fn.checkDates(end_date)}'
+
+    if indicator:
+        d['indicator'] = f'/indicator/{(fn.stringOrList(indicator))}'
+    
+    if country:
+        d['country'] = f'/country/{(fn.stringOrList(country))}'
+
+    if country and indicator:
+        d['indicator'] = f'/{fn.stringOrList(indicator)}'
+
+
+    api_url_request = "%s%s%s%s%s%s%s%s" % (d['url_base'], d['country'],d['indicator'], d['key'],d['limit'],d['start'],d['start_date'],d['end_date']) 
+    # print(api_url_request)
+    return fn.dataRequest(api_request=api_url_request, output_type=output_type)
+
+
+
+
```

### Comparing `tradingeconomics-4.2.8/tradingeconomics/stream.py` & `tradingeconomics-4.2.9/tradingeconomics/stream.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-import websocket
-import ssl
-
-import json
-from pprint import pprint
-from time import sleep
-import datetime as dt
-import threading
-from . import glob
-
-  
-
-te_url = "wss://stream.tradingeconomics.com"
-
-
-reconnect_timeout = 60
-function_to_restart = ["", ""]
-
-
-def on_error(ws, error):
-    print(error)
-
-def on_open(ws):
-    print("+++ Socket is open!")
-    for ev in glob._event:
-        print("+++ Subscribe to {0}".format(ev))
-        ws.send(json.dumps({'topic': 'subscribe', 'to': ev}) )
-
-def build_url():
-    return te_url + "?client=" + glob.apikey + "&app=python&token=20171116"
-
-def start_socket(on_message_client, *args):  
-    def _on_message(web_sock, message):
-        """ 
-            made so we do not have to reinitialize connection
-        """
-        t = threading.Thread(target=on_message_client, args=(web_sock, message))
-        t.start()
-       
-      
-    def _on_close(web_sock):
-        if (function_to_restart[1]) :
-            t = threading.Thread(target=function_to_restart[1], args=(web_sock, json.dumps({"msg" : "CLOSING"})))
-            t.start()
-        print("### closed ### reconnect in " + str(reconnect_timeout) + " seconds")
-        sleep(reconnect_timeout)
-        start_socket(function_to_restart[0]) 
-
-    
-    ws = websocket.WebSocketApp(build_url(),
-                              on_message = _on_message,
-                              on_error = on_error,
-                              on_close = _on_close)
-    
-    ws.on_open = on_open
-    ws.run_forever(sslopt={"cert_reqs": ssl.CERT_NONE})
-    ws.close()
-    
-
-def run(on_message_client, *args): ##passing on args ('on_close_client')
-
-    websocket.enableTrace(True)
-    function_to_restart[0] = on_message_client
-    
-    if (args):
-        function_to_restart[1] = args[0]
-        start_socket(function_to_restart[0], function_to_restart[1])
-    else:
-        start_socket(function_to_restart[0])
-    
-
+import websocket
+import ssl
+
+import json
+from pprint import pprint
+from time import sleep
+import datetime as dt
+import threading
+from . import glob
+
+  
+
+te_url = "wss://stream.tradingeconomics.com"
+
+
+reconnect_timeout = 60
+function_to_restart = ["", ""]
+
+
+def on_error(ws, error):
+    print(error)
+
+def on_open(ws):
+    print("+++ Socket is open!")
+    for ev in glob._event:
+        print("+++ Subscribe to {0}".format(ev))
+        ws.send(json.dumps({'topic': 'subscribe', 'to': ev}) )
+
+def build_url():
+    return te_url + "?client=" + glob.apikey + "&app=python&token=20171116"
+
+def start_socket(on_message_client, *args):  
+    def _on_message(web_sock, message):
+        """ 
+            made so we do not have to reinitialize connection
+        """
+        t = threading.Thread(target=on_message_client, args=(web_sock, message))
+        t.start()
+       
+      
+    def _on_close(web_sock):
+        if (function_to_restart[1]) :
+            t = threading.Thread(target=function_to_restart[1], args=(web_sock, json.dumps({"msg" : "CLOSING"})))
+            t.start()
+        print("### closed ### reconnect in " + str(reconnect_timeout) + " seconds")
+        sleep(reconnect_timeout)
+        start_socket(function_to_restart[0]) 
+
+    
+    ws = websocket.WebSocketApp(build_url(),
+                              on_message = _on_message,
+                              on_error = on_error,
+                              on_close = _on_close)
+    
+    ws.on_open = on_open
+    ws.run_forever(sslopt={"cert_reqs": ssl.CERT_NONE})
+    ws.close()
+    
+
+def run(on_message_client, *args): ##passing on args ('on_close_client')
+
+    websocket.enableTrace(True)
+    function_to_restart[0] = on_message_client
+    
+    if (args):
+        function_to_restart[1] = args[0]
+        start_socket(function_to_restart[0], function_to_restart[1])
+    else:
+        start_socket(function_to_restart[0])
+    
+
```

### Comparing `tradingeconomics-4.2.8/tradingeconomics/worldBank.py` & `tradingeconomics-4.2.9/tradingeconomics/worldBank.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,284 +1,284 @@
-import json 
-import urllib 
-import pandas as pd
-import sys
-from datetime import *
-from . import functions as fn
-from . import glob
-import ssl
-
-
-PY3 = sys.version_info[0] == 3
-
-if PY3: # Python 3+
-    from urllib.request import urlopen
-    from urllib.parse import quote
-else: # Python 2.X
-    from urllib import urlopen
-    from urllib import quote
-
-
-class ParametersError(ValueError):
-    pass
-
-class CredentialsError(ValueError):
-    pass
-
-class LoginError(AttributeError):
-    pass
-
-class WebRequestError(ValueError):
-    pass
-
-
-def checkSeriesCode(linkAPI, series_code):
-    linkAPI = 'https://api.tradingeconomics.com/worldBank/indicator'     
-    if series_code == None:
-        linkAPI += '?c=' + glob.apikey + '&s=' + quote(str(series_code)) 
-    else:
-        linkAPI += '?c=' + glob.apikey + '&s=' + quote("".join(series_code)) 
-       
-    return linkAPI  
-        
-def checkPageNumber(linkAPI, page_number):
-    if page_number != None:
-        linkAPI +=  '/{0}'.format(page_number) 
-    return linkAPI
-
-def checkCountry(linkAPI, country):
-    linkAPI = 'https://api.tradingeconomics.com/worldBank/country/'       
-    if type(country) is str:
-        linkAPI += quote(str(country), safe='')
-    else:
-        linkAPI += quote(",".join(country), safe='')
-        
-    return linkAPI
-
-def checkIndicator(linkAPI, indicator): 
-    linkAPI = 'https://api.tradingeconomics.com/worldBank/indicator/'     
-    if type(indicator) is str:
-        linkAPI +=  quote(str(indicator), safe='')
-    else:
-        linkAPI += quote(",".join(str(indicator), safe=''))
-    
-    return linkAPI
- 
-    
-
-def getWBCategories(category = None, page_number = None, output_type = None):
-    """
-    Return a list of all categories, categories by page number.
-    =================================================================================
-
-    Parameters:
-    -----------
-    categories:list.
-             List of strings for all categories and list of categories by page number.
-             All categories, for example:
-                category = None
-             Several categories or one category, for example:
-                category = ['education', 'agriculture']
-                category = 'education'
-             categories by page, for example:
-                category = 'education', page_number = 3
-                category = ['education', 'agriculture'], page_number = 5   
-    output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web. 
-
-    Notes
-    -----
-    All parameters are optional. Without parameters a list of all categories will be provided. 
-
-    Example
-    -------
-    getWBCategories(category = None, output_type = None)
-
-    getWBCategories(category = ['education', 'agriculture'], output_type = None)
-    """          
-    url = ''
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-    if category:
-        url = 'https://api.tradingeconomics.com/worldBank/category/' + quote(str(category), safe='')
-    else: 
-        url = 'https://api.tradingeconomics.com/worldBank/categories'
-    
-    if category == None:
-        linkAPI = 'https://api.tradingeconomics.com/worldBank/categories'
-    else:
-        linkAPI = 'https://api.tradingeconomics.com/worldBank/category/' + quote(str(category), safe='')
-    
-    if page_number != None:
-        linkAPI = checkPageNumber(linkAPI, page_number)
-     
-    try:
-        linkAPI += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-    
-    try:
-        # print(linkAPI)
-        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
-    except Exception as e:
-        print(e) 
-        
-
-def getWBIndicator(series_code = None, url = None, output_type = None):
-    """
-    Detailed information about specific indicator for all countries using a series 
-    code or url.
-    =================================================================================
-
-    Parameters:
-    -----------
-    series_code:list.
-             List of strings of indicators by series code.
-             sring of indicator by country using it's url.
-             Specific indicator and country by using series code, for example:
-                series_code = 'usa.fr.inr.rinr'(symbol used by TE for a country)
-    Url:string.            
-             Specific indicator and country by using url, for example:
-                url = '/united-states/real-interest-rate-percent-wb-data.html'             
-    output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web. 
-
-    Notes
-    -----
-    A series code or url is required. 
-
-    Example
-    -------
-
-    getWBIndicator(series_code = 'usa.fr.inr.rinr', url = None, output_type = None)
-
-    getWBIndicator(series_code = None, url = '/united-states/real-interest-rate-percent-wb-data.html', output_type = None)
-    """          
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-   
-    linkAPI = 'https://api.tradingeconomics.com/worldBank/indicator/'  
-    if series_code == None and url == None:
-        return "Series code or url is required!"  
-
-    if series_code != None:
-        linkAPI = 'https://api.tradingeconomics.com/worldBank/indicator' + '?c=' + glob.apikey + '&s=' + quote(str(series_code), safe='')            
-    elif url != None:
-        linkAPI = 'https://api.tradingeconomics.com/worldBank/indicator' + '?c=' + glob.apikey + '&url=' + quote(str(url), safe='')
-         
-   
-    try:
-        # print(linkAPI)
-        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
-    except Exception as e:
-        print(e) 
-
-  
-def getWBCountry(country = None, page_number = None, output_type = None):
-    """
-    List of indicators available for a specific country (with pagination).
-    =================================================================================
-
-    Parameters:
-    -----------
-    country:list.
-             List of strings of indicators by country.
-             country, for example:
-                country = 'portugal'
-    page_number:            
-                country = 'portugal', page_number = 3               
-    output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web. 
-
-    Notes
-    -----
-    A country is required to get a list.
-
-    Example
-    -------
-    getWBCountry(country = 'portugal', output_type = None) # page_number is no longer needed!
-    """ 
-    linkAPI = 'https://api.tradingeconomics.com/worldBank/country/'          
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-  
-    if country == None:
-        return "A country is required!" 
-    else:
-        linkAPI = checkCountry(linkAPI, country)
-
-    if page_number != None:    
-        linkAPI = checkPageNumber(linkAPI, page_number)
-    
-    try:
-        linkAPI += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
-    
-    try:
-        # print(linkAPI)
-        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
-    except Exception as e:
-        print(e) 
-
-
-def getWBHistorical(series_code = None, output_type = None):
-    """
-    Historical data for a specific indicator.
-    =================================================================================
-
-    Parameters:
-    -----------
-    series_code:list.
-             List of historical data by country.
-             for example:
-                series_code = None
-                series_code = 'usa.fr.inr.rinr'            
-    output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web. 
-
-    Notes
-    -----
-    A series code is required.
-
-    Example
-    -------
-    
-    getWBHistorical(series_code = 'usa.fr.inr.rinr', output_type = None)
-    """          
-    try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
-    
-    linkAPI = 'https://api.tradingeconomics.com/worldBank/historical' 
-    
-    if series_code == None:
-        return "A series code is required!"
-    else:
-        linkAPI += '?c=' + glob.apikey + '&s=' + quote(str(series_code))   
-    
-    try:
-        # print(linkAPI)
-        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
-    except Exception as e:
-        print(e) 
-  
-    
+import json 
+import urllib 
+import pandas as pd
+import sys
+from datetime import *
+from . import functions as fn
+from . import glob
+import ssl
+
+
+PY3 = sys.version_info[0] == 3
+
+if PY3: # Python 3+
+    from urllib.request import urlopen
+    from urllib.parse import quote
+else: # Python 2.X
+    from urllib import urlopen
+    from urllib import quote
+
+
+class ParametersError(ValueError):
+    pass
+
+class CredentialsError(ValueError):
+    pass
+
+class LoginError(AttributeError):
+    pass
+
+class WebRequestError(ValueError):
+    pass
+
+
+def checkSeriesCode(linkAPI, series_code):
+    linkAPI = 'https://api.tradingeconomics.com/worldBank/indicator'     
+    if series_code == None:
+        linkAPI += '?c=' + glob.apikey + '&s=' + quote(str(series_code)) 
+    else:
+        linkAPI += '?c=' + glob.apikey + '&s=' + quote("".join(series_code)) 
+       
+    return linkAPI  
+        
+def checkPageNumber(linkAPI, page_number):
+    if page_number != None:
+        linkAPI +=  '/{0}'.format(page_number) 
+    return linkAPI
+
+def checkCountry(linkAPI, country):
+    linkAPI = 'https://api.tradingeconomics.com/worldBank/country/'       
+    if type(country) is str:
+        linkAPI += quote(str(country), safe='')
+    else:
+        linkAPI += quote(",".join(country), safe='')
+        
+    return linkAPI
+
+def checkIndicator(linkAPI, indicator): 
+    linkAPI = 'https://api.tradingeconomics.com/worldBank/indicator/'     
+    if type(indicator) is str:
+        linkAPI +=  quote(str(indicator), safe='')
+    else:
+        linkAPI += quote(",".join(str(indicator), safe=''))
+    
+    return linkAPI
+ 
+    
+
+def getWBCategories(category = None, page_number = None, output_type = None):
+    """
+    Return a list of all categories, categories by page number.
+    =================================================================================
+
+    Parameters:
+    -----------
+    categories:list.
+             List of strings for all categories and list of categories by page number.
+             All categories, for example:
+                category = None
+             Several categories or one category, for example:
+                category = ['education', 'agriculture']
+                category = 'education'
+             categories by page, for example:
+                category = 'education', page_number = 3
+                category = ['education', 'agriculture'], page_number = 5   
+    output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+
+    Notes
+    -----
+    All parameters are optional. Without parameters a list of all categories will be provided. 
+
+    Example
+    -------
+    getWBCategories(category = None, output_type = None)
+
+    getWBCategories(category = ['education', 'agriculture'], output_type = None)
+    """          
+    url = ''
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+    if category:
+        url = 'https://api.tradingeconomics.com/worldBank/category/' + quote(str(category), safe='')
+    else: 
+        url = 'https://api.tradingeconomics.com/worldBank/categories'
+    
+    if category == None:
+        linkAPI = 'https://api.tradingeconomics.com/worldBank/categories'
+    else:
+        linkAPI = 'https://api.tradingeconomics.com/worldBank/category/' + quote(str(category), safe='')
+    
+    if page_number != None:
+        linkAPI = checkPageNumber(linkAPI, page_number)
+     
+    try:
+        linkAPI += '?c=' + glob.apikey
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+    
+    try:
+        # print(linkAPI)
+        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
+    except Exception as e:
+        print(e) 
+        
+
+def getWBIndicator(series_code = None, url = None, output_type = None):
+    """
+    Detailed information about specific indicator for all countries using a series 
+    code or url.
+    =================================================================================
+
+    Parameters:
+    -----------
+    series_code:list.
+             List of strings of indicators by series code.
+             sring of indicator by country using it's url.
+             Specific indicator and country by using series code, for example:
+                series_code = 'usa.fr.inr.rinr'(symbol used by TE for a country)
+    Url:string.            
+             Specific indicator and country by using url, for example:
+                url = '/united-states/real-interest-rate-percent-wb-data.html'             
+    output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+
+    Notes
+    -----
+    A series code or url is required. 
+
+    Example
+    -------
+
+    getWBIndicator(series_code = 'usa.fr.inr.rinr', url = None, output_type = None)
+
+    getWBIndicator(series_code = None, url = '/united-states/real-interest-rate-percent-wb-data.html', output_type = None)
+    """          
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+   
+    linkAPI = 'https://api.tradingeconomics.com/worldBank/indicator/'  
+    if series_code == None and url == None:
+        return "Series code or url is required!"  
+
+    if series_code != None:
+        linkAPI = 'https://api.tradingeconomics.com/worldBank/indicator' + '?c=' + glob.apikey + '&s=' + quote(str(series_code), safe='')            
+    elif url != None:
+        linkAPI = 'https://api.tradingeconomics.com/worldBank/indicator' + '?c=' + glob.apikey + '&url=' + quote(str(url), safe='')
+         
+   
+    try:
+        # print(linkAPI)
+        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
+    except Exception as e:
+        print(e) 
+
+  
+def getWBCountry(country = None, page_number = None, output_type = None):
+    """
+    List of indicators available for a specific country (with pagination).
+    =================================================================================
+
+    Parameters:
+    -----------
+    country:list.
+             List of strings of indicators by country.
+             country, for example:
+                country = 'portugal'
+    page_number:            
+                country = 'portugal', page_number = 3               
+    output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+
+    Notes
+    -----
+    A country is required to get a list.
+
+    Example
+    -------
+    getWBCountry(country = 'portugal', output_type = None) # page_number is no longer needed!
+    """ 
+    linkAPI = 'https://api.tradingeconomics.com/worldBank/country/'          
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+  
+    if country == None:
+        return "A country is required!" 
+    else:
+        linkAPI = checkCountry(linkAPI, country)
+
+    if page_number != None:    
+        linkAPI = checkPageNumber(linkAPI, page_number)
+    
+    try:
+        linkAPI += '?c=' + glob.apikey
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+    
+    try:
+        # print(linkAPI)
+        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
+    except Exception as e:
+        print(e) 
+
+
+def getWBHistorical(series_code = None, output_type = None):
+    """
+    Historical data for a specific indicator.
+    =================================================================================
+
+    Parameters:
+    -----------
+    series_code:list.
+             List of historical data by country.
+             for example:
+                series_code = None
+                series_code = 'usa.fr.inr.rinr'            
+    output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+
+    Notes
+    -----
+    A series code is required.
+
+    Example
+    -------
+    
+    getWBHistorical(series_code = 'usa.fr.inr.rinr', output_type = None)
+    """          
+    try:
+        _create_unverified_https_context = ssl._create_unverified_context
+    except AttributeError:
+        pass
+    else:
+        ssl._create_default_https_context = _create_unverified_https_context
+    
+    linkAPI = 'https://api.tradingeconomics.com/worldBank/historical' 
+    
+    if series_code == None:
+        return "A series code is required!"
+    else:
+        linkAPI += '?c=' + glob.apikey + '&s=' + quote(str(series_code))   
+    
+    try:
+        # print(linkAPI)
+        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
+    except Exception as e:
+        print(e) 
+  
+
```

### Comparing `tradingeconomics-4.2.8/tradingeconomics.egg-info/PKG-INFO` & `tradingeconomics-4.2.9/tradingeconomics.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-Metadata-Version: 2.1
-Name: tradingeconomics
-Version: 4.2.8
-Summary: Trading Economics API
-Home-page: https://github.com/tradingeconomics/tradingeconomics-python
-Download-URL: https://github.com/tradingeconomics/tradingeconomics-python/tree/main/dist
-Author: Trading Economics
-Author-email: support@tradingeconomics.com
-License: MIT
-Keywords: tradingeconomics,data
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-=====================
-Trading Economics API
-=====================
-
-The Trading Economics Python package provides direct access to over 300,000 economic indicators, exchange rates, stock market indexes, government bond yields, and commodity prices. This package offers various request methods to query the Trading Economics databases and supports exporting data in XML, CSV, or JSON format. The API can be used to feed custom-developed applications, public websites, or off-the-shelf software.
-
-
-Installation
-----------------------------------------
-
-You can install the package using pip:
-
-    - pip install tradingeconomics
-
-
-Authentication
-----------------------------------------
-
-To use the Trading Economics API, you need to authenticate by providing your API key and secret:
-
-    - import tradingeconomics as te
-    - te.login('key:secret')
-
-
-Sample Usage
-----------------------------------------
-
-Here are some examples of how to use the Trading Economics Python package:
-
-    - te.getCalendarData()
-    - te.getIndicatorData(country=['mexico', 'sweden'], output_type='df')
-    - te.getMarketsData(marketsField='commodities')
-    - te.getMarketsBySymbol(symbols='aapl:us')
-    - te.getFinancialsData(symbol='aapl:us', output_type='df')
-
-
-GitHub Examples
-----------------------------------------
-
-You can find additional examples and usage instructions in the GitHub repository:
- - https://github.com/tradingeconomics/tradingeconomics-python/tree/main/examples
-
-
-Documentation
-----------------------------------------
-
-For detailed documentation and API reference, please visit the Trading Economics API documentation:
- - https://docs.tradingeconomics.com
+Metadata-Version: 2.1
+Name: tradingeconomics
+Version: 4.2.9
+Summary: Trading Economics API
+Home-page: https://github.com/tradingeconomics/tradingeconomics-python
+Download-URL: https://github.com/tradingeconomics/tradingeconomics-python/tree/main/dist
+Author: Trading Economics
+Author-email: support@tradingeconomics.com
+License: MIT
+Keywords: tradingeconomics,data
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.2
+Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+=====================
+Trading Economics API
+=====================
+
+The Trading Economics Python package provides direct access to over 300,000 economic indicators, exchange rates, stock market indexes, government bond yields, and commodity prices. This package offers various request methods to query the Trading Economics databases and supports exporting data in XML, CSV, or JSON format. The API can be used to feed custom-developed applications, public websites, or off-the-shelf software.
+
+
+Installation
+----------------------------------------
+
+You can install the package using pip:
+
+    - pip install tradingeconomics
+
+
+Authentication
+----------------------------------------
+
+To use the Trading Economics API, you need to authenticate by providing your API key and secret:
+
+    - import tradingeconomics as te
+    - te.login('key:secret')
+
+
+Sample Usage
+----------------------------------------
+
+Here are some examples of how to use the Trading Economics Python package:
+
+    - te.getCalendarData()
+    - te.getIndicatorData(country=['mexico', 'sweden'], output_type='df')
+    - te.getMarketsData(marketsField='commodities')
+    - te.getMarketsBySymbol(symbols='aapl:us')
+    - te.getFinancialsData(symbol='aapl:us', output_type='df')
+
+
+GitHub Examples
+----------------------------------------
+
+You can find additional examples and usage instructions in the GitHub repository:
+ - https://github.com/tradingeconomics/tradingeconomics-python/tree/main/examples
+
+
+Documentation
+----------------------------------------
+
+For detailed documentation and API reference, please visit the Trading Economics API documentation:
+ - https://docs.tradingeconomics.com
```

### Comparing `tradingeconomics-4.2.8/tradingeconomics.egg-info/SOURCES.txt` & `tradingeconomics-4.2.9/tradingeconomics.egg-info/SOURCES.txt`

 * *Files identical despite different names*


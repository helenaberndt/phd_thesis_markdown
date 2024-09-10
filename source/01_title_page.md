<!--
  Zentrale Variablen:
  Workaround bzw. Rückgriff auf LaTex-Befehle, um zentrale Werte immer wieder verwenden zu können.
-->


<!--
%% Abschlussarbeit
-->
\newcommand{\titel}{Titel der Abschlussarbeit}
\newcommand{\datum}{xx.xx.xxxx}
<!--
% Autor_in
-->
\newcommand{\aVorname}{Helena}
\newcommand{\aNachname}{Berndt}
\newcommand{\aGeburtsdatum}{01.03.2002}
\newcommand{\aInstitution}{Hochschule München}
\newcommand{\aStudiengruppe}{IF7}
\newcommand{\aSemester}{WS 2024/2025}

\newcommand{\aName}{\aVorname\space \aNachname}
<!--
% Prüfer_in
-->
\newcommand{\pTitle}{Prof. Dr.}
\newcommand{\pVorname}{Lars}
\newcommand{\pNachname}{Wischhof}
\newcommand{\pInstitution}{Hochschule München}
<!--
% Betreuer_in
-->
\newcommand{\bTitle}{}
\newcommand{\bVorname}{Daniel}
\newcommand{\bNachname}{Abram}
\newcommand{\bInstitution}{BMW Group}

\title{\titel}
\author{\aName}

<!--
  Titelseite
-->

\begin{titlepage}
    \begin{center}

        \includegraphics[width=1\textwidth]{style/hm-fk07_logo.jpg}

        \vspace*{1.0cm}

        \LARGE
        \titel

        \vspace{1.5cm}

        \Large
        \aName

        \vspace{0.5cm}

        \normalsize
        Bachelorarbeit Informatik

        \vfill

        \normalsize
        Prüfer:\\
        \pTitle\space \pVorname\space \pNachname,\space \pInstitution

        \vspace{0.5cm}

        Firmenlogo
        % \includegraphics[width=0.4\textwidth]{style/firmenlogo.png}

        \normalsize
        Betreuer:\\
        \bTitle\space \bVorname\space \bNachname,\space \bInstitution

        % Abgabedatum
        \datum

    \end{center}
\end{titlepage}
